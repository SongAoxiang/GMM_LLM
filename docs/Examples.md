
# Usage Examples

This section provides hands-on examples to help you integrate **Open WebUI** into your own applications. All requests assume the backend is running locally on port `8080`. Adjust the base-URL accordingly if you deploy elsewhere.

## 1. Authentication – obtain a JSON Web Token (JWT)

```bash
curl -X POST http://localhost:8080/api/v1/auths/signin      -H 'Content-Type: application/json'      -d '{"email": "demo@example.com", "password": "secret"}'
```

The response contains a `token` property which must be passed in the `Authorization` header for all protected endpoints:

```http
Authorization: Bearer <token_here>
```

## 2. List available AI models

```bash
curl -H 'Authorization: Bearer <token>'      http://localhost:8080/api/v1/models/
```

## 3. Start a new chat and stream completions

```bash
# Create chat shell (returns chat_id)
curl -X POST -H 'Authorization: Bearer <token>'      -H 'Content-Type: application/json'      -d '{"title": "My first chat"}'      http://localhost:8080/api/v1/chats/new

# Send a user message & receive streamed response
curl -X POST -H 'Authorization: Bearer <token>'      -H 'Accept: text/event-stream'      -H 'Content-Type: application/json'      -d '{"chat_id": "<chat_id>", "content": "Hello!"}'      http://localhost:8080/api/chat/completions
```

## 4. Generate an image

```bash
curl -X POST -H 'Authorization: Bearer <token>'      -H 'Content-Type: application/json'      -d '{"prompt": "Astronaut riding a horse in space"}'      http://localhost:8080/api/v1/images/generations
```

## 5. Frontend component example

```svelte
<script lang="ts">
  import Chat from '$lib/components/chat/Chat.svelte';
</script>

<Chat chatId={"abc123"} />
```

