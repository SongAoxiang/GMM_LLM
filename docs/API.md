# Public REST API Documentation

This document lists all available HTTP endpoints exposed by the **Open WebUI** backend. Each table is grouped by logical router/component as defined in the source code.

> Tip: run the backend in development mode and open `/docs` in the browser to explore the interactive Swagger-UI.

## Audio Routes

Method | Path
--- | ---
GET | `/api/v1/audio/config`
POST | `/api/v1/audio/config/update`
GET | `/api/v1/audio/models`
POST | `/api/v1/audio/speech`
POST | `/api/v1/audio/transcriptions`
GET | `/api/v1/audio/voices`

## Auths Routes

Method | Path
--- | ---
GET | `/api/v1/auths/`
POST | `/api/v1/auths/add`
GET | `/api/v1/auths/admin/config`
POST | `/api/v1/auths/admin/config`
GET | `/api/v1/auths/admin/config/ldap`
POST | `/api/v1/auths/admin/config/ldap`
GET | `/api/v1/auths/admin/config/ldap/server`
POST | `/api/v1/auths/admin/config/ldap/server`
GET | `/api/v1/auths/admin/details`
POST | `/api/v1/auths/api_key`
DELETE | `/api/v1/auths/api_key`
GET | `/api/v1/auths/api_key`
POST | `/api/v1/auths/ldap`
POST | `/api/v1/auths/signin`
GET | `/api/v1/auths/signout`
POST | `/api/v1/auths/signup`
POST | `/api/v1/auths/update/password`
POST | `/api/v1/auths/update/profile`

## Channels Routes

Method | Path
--- | ---
GET | `/api/v1/channels/`
POST | `/api/v1/channels/create`
GET | `/api/v1/channels/{id}`
DELETE | `/api/v1/channels/{id}/delete`
GET | `/api/v1/channels/{id}/messages`
POST | `/api/v1/channels/{id}/messages/post`
GET | `/api/v1/channels/{id}/messages/{message_id}`
DELETE | `/api/v1/channels/{id}/messages/{message_id}/delete`
POST | `/api/v1/channels/{id}/messages/{message_id}/reactions/add`
POST | `/api/v1/channels/{id}/messages/{message_id}/reactions/remove`
POST | `/api/v1/channels/{id}/update`

## Chats Routes

Method | Path
--- | ---
GET | `/api/v1/chats/`
DELETE | `/api/v1/chats/`
GET | `/api/v1/chats/all`
GET | `/api/v1/chats/all/archived`
GET | `/api/v1/chats/all/db`
GET | `/api/v1/chats/all/tags`
POST | `/api/v1/chats/archive/all`
GET | `/api/v1/chats/archived`
GET | `/api/v1/chats/folder/{folder_id}`
POST | `/api/v1/chats/import`
GET | `/api/v1/chats/list`
GET | `/api/v1/chats/list/user/{user_id}`
POST | `/api/v1/chats/new`
GET | `/api/v1/chats/pinned`
GET | `/api/v1/chats/search`
GET | `/api/v1/chats/share/{share_id}`
POST | `/api/v1/chats/tags`
GET | `/api/v1/chats/{id}`
POST | `/api/v1/chats/{id}`
DELETE | `/api/v1/chats/{id}`
POST | `/api/v1/chats/{id}/archive`
POST | `/api/v1/chats/{id}/clone`
POST | `/api/v1/chats/{id}/clone/shared`
POST | `/api/v1/chats/{id}/folder`
POST | `/api/v1/chats/{id}/messages/{message_id}`
POST | `/api/v1/chats/{id}/messages/{message_id}/event`
POST | `/api/v1/chats/{id}/pin`
GET | `/api/v1/chats/{id}/pinned`
POST | `/api/v1/chats/{id}/share`
DELETE | `/api/v1/chats/{id}/share`
GET | `/api/v1/chats/{id}/tags`
POST | `/api/v1/chats/{id}/tags`
DELETE | `/api/v1/chats/{id}/tags`
DELETE | `/api/v1/chats/{id}/tags/all`

## Configs Routes

Method | Path
--- | ---
POST | `/api/v1/configs/banners`
GET | `/api/v1/configs/banners`
GET | `/api/v1/configs/code_execution`
POST | `/api/v1/configs/code_execution`
GET | `/api/v1/configs/direct_connections`
POST | `/api/v1/configs/direct_connections`
GET | `/api/v1/configs/export`
POST | `/api/v1/configs/import`
GET | `/api/v1/configs/models`
POST | `/api/v1/configs/models`
POST | `/api/v1/configs/suggestions`
GET | `/api/v1/configs/tool_servers`
POST | `/api/v1/configs/tool_servers`
POST | `/api/v1/configs/tool_servers/verify`

## Evaluations Routes

Method | Path
--- | ---
GET | `/config`
POST | `/config`
POST | `/feedback`
GET | `/feedback/{id}`
POST | `/feedback/{id}`
DELETE | `/feedback/{id}`
DELETE | `/feedbacks`
GET | `/feedbacks/all`
DELETE | `/feedbacks/all`
GET | `/feedbacks/all/export`
GET | `/feedbacks/user`

## Files Routes

Method | Path
--- | ---
POST | `/api/v1/files/`
GET | `/api/v1/files/`
DELETE | `/api/v1/files/all`
GET | `/api/v1/files/search`
GET | `/api/v1/files/{id}`
DELETE | `/api/v1/files/{id}`
GET | `/api/v1/files/{id}/content`
GET | `/api/v1/files/{id}/content/html`
GET | `/api/v1/files/{id}/content/{file_name}`
GET | `/api/v1/files/{id}/data/content`
POST | `/api/v1/files/{id}/data/content/update`

## Folders Routes

Method | Path
--- | ---
GET | `/api/v1/folders/`
POST | `/api/v1/folders/`
GET | `/api/v1/folders/{id}`
DELETE | `/api/v1/folders/{id}`
POST | `/api/v1/folders/{id}/update`
POST | `/api/v1/folders/{id}/update/expanded`
POST | `/api/v1/folders/{id}/update/parent`

## Functions Routes

Method | Path
--- | ---
GET | `/api/v1/functions/`
POST | `/api/v1/functions/create`
GET | `/api/v1/functions/export`
GET | `/api/v1/functions/id/{id}`
DELETE | `/api/v1/functions/id/{id}/delete`
POST | `/api/v1/functions/id/{id}/toggle`
POST | `/api/v1/functions/id/{id}/toggle/global`
POST | `/api/v1/functions/id/{id}/update`
GET | `/api/v1/functions/id/{id}/valves`
GET | `/api/v1/functions/id/{id}/valves/spec`
POST | `/api/v1/functions/id/{id}/valves/update`
GET | `/api/v1/functions/id/{id}/valves/user`
GET | `/api/v1/functions/id/{id}/valves/user/spec`
POST | `/api/v1/functions/id/{id}/valves/user/update`

## Groups Routes

Method | Path
--- | ---
GET | `/api/v1/groups/`
POST | `/api/v1/groups/create`
GET | `/api/v1/groups/id/{id}`
DELETE | `/api/v1/groups/id/{id}/delete`
POST | `/api/v1/groups/id/{id}/update`

## Images Routes

Method | Path
--- | ---
GET | `/api/v1/images/config`
POST | `/api/v1/images/config/update`
GET | `/api/v1/images/config/url/verify`
POST | `/api/v1/images/generations`
GET | `/api/v1/images/image/config`
POST | `/api/v1/images/image/config/update`
GET | `/api/v1/images/models`

## Knowledge Routes

Method | Path
--- | ---
GET | `/api/v1/knowledge/`
POST | `/api/v1/knowledge/create`
GET | `/api/v1/knowledge/list`
POST | `/api/v1/knowledge/reindex`
GET | `/api/v1/knowledge/{id}`
DELETE | `/api/v1/knowledge/{id}/delete`
POST | `/api/v1/knowledge/{id}/file/add`
POST | `/api/v1/knowledge/{id}/file/remove`
POST | `/api/v1/knowledge/{id}/file/update`
POST | `/api/v1/knowledge/{id}/files/batch/add`
POST | `/api/v1/knowledge/{id}/reset`
POST | `/api/v1/knowledge/{id}/update`

## Memories Routes

Method | Path
--- | ---
GET | `/api/v1/memories/`
POST | `/api/v1/memories/add`
DELETE | `/api/v1/memories/delete/user`
GET | `/api/v1/memories/ef`
POST | `/api/v1/memories/query`
POST | `/api/v1/memories/reset`
DELETE | `/api/v1/memories/{memory_id}`
POST | `/api/v1/memories/{memory_id}/update`

## Models Routes

Method | Path
--- | ---
GET | `/api/v1/models/`
GET | `/api/v1/models/base`
POST | `/api/v1/models/create`
DELETE | `/api/v1/models/delete/all`
GET | `/api/v1/models/model`
DELETE | `/api/v1/models/model/delete`
POST | `/api/v1/models/model/toggle`
POST | `/api/v1/models/model/update`

## Notes Routes

Method | Path
--- | ---
GET | `/api/v1/notes/`
POST | `/api/v1/notes/create`
GET | `/api/v1/notes/list`
GET | `/api/v1/notes/{id}`
DELETE | `/api/v1/notes/{id}/delete`
POST | `/api/v1/notes/{id}/update`

## Ollama Routes

Method | Path
--- | ---
HEAD | `/ollama/`
GET | `/ollama/`
POST | `/ollama/api/chat`
POST | `/ollama/api/chat/{url_idx}`
POST | `/ollama/api/copy`
POST | `/ollama/api/copy/{url_idx}`
POST | `/ollama/api/create`
POST | `/ollama/api/create/{url_idx}`
DELETE | `/ollama/api/delete`
DELETE | `/ollama/api/delete/{url_idx}`
POST | `/ollama/api/embed`
POST | `/ollama/api/embed/{url_idx}`
POST | `/ollama/api/embeddings`
POST | `/ollama/api/embeddings/{url_idx}`
POST | `/ollama/api/generate`
POST | `/ollama/api/generate/{url_idx}`
GET | `/ollama/api/ps`
POST | `/ollama/api/pull`
POST | `/ollama/api/pull/{url_idx}`
DELETE | `/ollama/api/push`
DELETE | `/ollama/api/push/{url_idx}`
POST | `/ollama/api/show`
GET | `/ollama/api/tags`
GET | `/ollama/api/tags/{url_idx}`
GET | `/ollama/api/version`
GET | `/ollama/api/version/{url_idx}`
GET | `/ollama/config`
POST | `/ollama/config/update`
POST | `/ollama/models/download`
POST | `/ollama/models/download/{url_idx}`
POST | `/ollama/models/upload`
POST | `/ollama/models/upload/{url_idx}`
POST | `/ollama/v1/chat/completions`
POST | `/ollama/v1/chat/completions/{url_idx}`
POST | `/ollama/v1/completions`
POST | `/ollama/v1/completions/{url_idx}`
GET | `/ollama/v1/models`
GET | `/ollama/v1/models/{url_idx}`
POST | `/ollama/verify`

## Openai Routes

Method | Path
--- | ---
POST | `/openai/audio/speech`
POST | `/openai/chat/completions`
GET | `/openai/config`
POST | `/openai/config/update`
GET | `/openai/models`
GET | `/openai/models/{url_idx}`
POST | `/openai/verify`

## Pipelines Routes

Method | Path
--- | ---
GET | `/api/v1/pipelines/`
POST | `/api/v1/pipelines/add`
DELETE | `/api/v1/pipelines/delete`
GET | `/api/v1/pipelines/list`
POST | `/api/v1/pipelines/upload`
GET | `/api/v1/pipelines/{pipeline_id}/valves`
GET | `/api/v1/pipelines/{pipeline_id}/valves/spec`
POST | `/api/v1/pipelines/{pipeline_id}/valves/update`

## Prompts Routes

Method | Path
--- | ---
GET | `/api/v1/prompts/`
GET | `/api/v1/prompts/command/{command}`
DELETE | `/api/v1/prompts/command/{command}/delete`
POST | `/api/v1/prompts/command/{command}/update`
POST | `/api/v1/prompts/create`
GET | `/api/v1/prompts/list`

## Retrieval Routes

Method | Path
--- | ---
GET | `/api/v1/retrieval/`
GET | `/api/v1/retrieval/config`
POST | `/api/v1/retrieval/config/update`
POST | `/api/v1/retrieval/delete`
GET | `/api/v1/retrieval/ef/{text}`
GET | `/api/v1/retrieval/embedding`
POST | `/api/v1/retrieval/embedding/update`
POST | `/api/v1/retrieval/process/file`
POST | `/api/v1/retrieval/process/files/batch`
POST | `/api/v1/retrieval/process/text`
POST | `/api/v1/retrieval/process/web`
POST | `/api/v1/retrieval/process/web/search`
POST | `/api/v1/retrieval/process/youtube`
POST | `/api/v1/retrieval/query/collection`
POST | `/api/v1/retrieval/query/doc`
POST | `/api/v1/retrieval/reset/db`
POST | `/api/v1/retrieval/reset/uploads`

## Tasks Routes

Method | Path
--- | ---
POST | `/api/v1/tasks/auto/completions`
GET | `/api/v1/tasks/config`
POST | `/api/v1/tasks/config/update`
POST | `/api/v1/tasks/emoji/completions`
POST | `/api/v1/tasks/image_prompt/completions`
POST | `/api/v1/tasks/moa/completions`
POST | `/api/v1/tasks/queries/completions`
POST | `/api/v1/tasks/tags/completions`
POST | `/api/v1/tasks/title/completions`

## Tools Routes

Method | Path
--- | ---
GET | `/api/v1/tools/`
POST | `/api/v1/tools/create`
GET | `/api/v1/tools/export`
GET | `/api/v1/tools/id/{id}`
DELETE | `/api/v1/tools/id/{id}/delete`
POST | `/api/v1/tools/id/{id}/update`
GET | `/api/v1/tools/id/{id}/valves`
GET | `/api/v1/tools/id/{id}/valves/spec`
POST | `/api/v1/tools/id/{id}/valves/update`
GET | `/api/v1/tools/id/{id}/valves/user`
GET | `/api/v1/tools/id/{id}/valves/user/spec`
POST | `/api/v1/tools/id/{id}/valves/user/update`
GET | `/api/v1/tools/list`

## Users Routes

Method | Path
--- | ---
GET | `/api/v1/users/`
GET | `/api/v1/users/all`
GET | `/api/v1/users/default/permissions`
POST | `/api/v1/users/default/permissions`
GET | `/api/v1/users/groups`
GET | `/api/v1/users/permissions`
POST | `/api/v1/users/update/role`
GET | `/api/v1/users/user/info`
POST | `/api/v1/users/user/info/update`
GET | `/api/v1/users/user/settings`
POST | `/api/v1/users/user/settings/update`
GET | `/api/v1/users/{user_id}`
DELETE | `/api/v1/users/{user_id}`
POST | `/api/v1/users/{user_id}/update`

## Utils Routes

Method | Path
--- | ---
POST | `/api/v1/utils/code/execute`
POST | `/api/v1/utils/code/format`
GET | `/api/v1/utils/db/download`
GET | `/api/v1/utils/gravatar`
GET | `/api/v1/utils/litellm/config`
POST | `/api/v1/utils/markdown`
POST | `/api/v1/utils/pdf`
