# Frontend Components

This section lists reusable Svelte components available in the **Open WebUI** frontend. Import them from `src/lib/components` or one of its sub-folders.

Basic usage pattern:
```svelte
<script lang="ts">
  import { ComponentName } from '$lib/components/<category>';
</script>

<ComponentName propA={value} />
```

---

## Admin Components

- **AddGroupModal**
- **AddUserModal**
- **ArenaModelModal**
- **Audio**
- **CodeExecution**
- **ConfigureModelsModal**
- **Connections**
- **Database**
- **Display**
- **Documents**
- **EditGroupModal**
- **EditUserModal**
- **Evaluations**
- **Evaluations**
- **FeedbackMenu**
- **Feedbacks**
- **FunctionEditor**
- **FunctionMenu**
- **Functions**
- **General**
- **GroupItem**
- **Groups**
- **Images**
- **Interface**
- **Leaderboard**
- **ManageModelsModal**
- **ManageMultipleOllama**
- **ManageOllama**
- **ManageOllamaModal**
- **Model**
- **ModelList**
- **ModelMenu**
- **Models**
- **OllamaConnection**
- **OpenAIConnection**
- **Permissions**
- **Pipelines**
- **Settings**
- **Tools**
- **UserChatsModal**
- **UserList**
- **Users**
- **Users**
- **WebSearch**

## App Components

- **AppSidebar**

## Channel Components

- **Channel**
- **InputMenu**
- **Message**
- **MessageInput**
- **Messages**
- **Navbar**
- **ProfilePreview**
- **ReactionPicker**
- **Thread**

## Chat Components

- **About**
- **Account**
- **AddMemoryModal**
- **AdvancedParams**
- **AlertRenderer**
- **Artifacts**
- **Audio**
- **CallOverlay**
- **Chat**
- **ChatControls**
- **ChatPlaceholder**
- **Chats**
- **Citations**
- **CitationsModal**
- **CodeBlock**
- **CodeExecutionModal**
- **CodeExecutions**
- **Commands**
- **Connection**
- **Connection**
- **Connections**
- **ContentRenderer**
- **Controls**
- **EditMemoryModal**
- **Error**
- **FilesOverlay**
- **FloatingButtons**
- **Flow**
- **General**
- **HTMLToken**
- **InputMenu**
- **Interface**
- **KatexRenderer**
- **Knowledge**
- **ManageModal**
- **Markdown**
- **MarkdownInlineTokens**
- **MarkdownTokens**
- **Message**
- **MessageInput**
- **Messages**
- **ModelSelector**
- **Models**
- **MultiResponseMessages**
- **Name**
- **Navbar**
- **Node**
- **Overview**
- **Personalization**
- **Placeholder**
- **ProfileImage**
- **Prompts**
- **RateComment**
- **ResponseMessage**
- **Selector**
- **SettingsModal**
- **ShareChatModal**
- **ShortcutsModal**
- **Skeleton**
- **Source**
- **Suggestions**
- **TagChatModal**
- **Tags**
- **ToolServersModal**
- **Tools**
- **UpdatePassword**
- **UserMessage**
- **Valves**
- **VideoInputMenu**
- **VoiceRecording**
- **WebSearchResults**

## Common Components

- **Badge**
- **Banner**
- **Checkbox**
- **CodeEditor**
- **Collapsible**
- **ConfirmDialog**
- **DragGhost**
- **Drawer**
- **Dropdown**
- **FileItem**
- **FileItemModal**
- **Folder**
- **Image**
- **ImagePreview**
- **Loader**
- **Marquee**
- **Modal**
- **Overlay**
- **Pagination**
- **RichTextInput**
- **SVGPanZoom**
- **Selector**
- **SensitiveInput**
- **Sidebar**
- **SlideShow**
- **Spinner**
- **Switch**
- **TagInput**
- **TagList**
- **Tags**
- **Textarea**
- **Tooltip**
- **Valves**

## Icons Components

- **AdjustmentsHorizontal**
- **ArchiveBox**
- **ArrowDownTray**
- **ArrowLeft**
- **ArrowPath**
- **ArrowRight**
- **ArrowRightCircle**
- **ArrowUpCircle**
- **ArrowUpTray**
- **ArrowUturnLeft**
- **ArrowUturnRight**
- **ArrowsPointingOut**
- **Bars3BottomLeft**
- **BarsArrowUp**
- **Bolt**
- **BookOpen**
- **Bookmark**
- **BookmarkSlash**
- **Calendar**
- **CalendarSolid**
- **CameraSolid**
- **ChartBar**
- **ChatBubble**
- **ChatBubbleOval**
- **ChatBubbleOvalEllipsis**
- **ChatBubbles**
- **Check**
- **ChevronDown**
- **ChevronLeft**
- **ChevronRight**
- **ChevronUp**
- **ChevronUpDown**
- **Clipboard**
- **CloudArrowUp**
- **Cog6**
- **Cog6Solid**
- **CommandLine**
- **CommandLineSolid**
- **Cube**
- **CursorArrowRays**
- **Document**
- **DocumentArrowDown**
- **DocumentArrowUp**
- **DocumentArrowUpSolid**
- **DocumentChartBar**
- **DocumentDuplicate**
- **Download**
- **EllipsisHorizontal**
- **EllipsisVertical**
- **Eye**
- **EyeSlash**
- **FaceSmile**
- **FloppyDisk**
- **FolderOpen**
- **GarbageBin**
- **GlobeAlt**
- **GlobeAltSolid**
- **Headphone**
- **Heart**
- **Home**
- **Info**
- **Keyboard**
- **Lifebuoy**
- **LightBlub**
- **LightBulb**
- **Link**
- **LockClosed**
- **MagnifyingGlass**
- **Map**
- **MenuLines**
- **Merge**
- **Mic**
- **MicSolid**
- **Minus**
- **Pencil**
- **PencilSolid**
- **PencilSquare**
- **Photo**
- **PhotoSolid**
- **Plus**
- **QuestionMarkCircle**
- **Reset**
- **Search**
- **Share**
- **Sparkles**
- **SparklesSolid**
- **Star**
- **User**
- **UserCircleSolid**
- **UserPlusSolid**
- **Users**
- **UsersSolid**
- **Wrench**
- **WrenchSolid**
- **XMark**

## Layout Components

- **AccountPending**
- **ArchivedChatsModal**
- **ChannelItem**
- **ChannelModal**
- **ChatItem**
- **ChatMenu**
- **FolderMenu**
- **Folders**
- **Help**
- **HelpMenu**
- **Menu**
- **Navbar**
- **RecursiveFolder**
- **SearchInput**
- **SearchModal**
- **Sidebar**
- **UpdateInfoToast**
- **UserMenu**

## Notes Components

- **NoteEditor**
- **NoteMenu**
- **Notes**
- **RecordMenu**

## Playground Components

- **Chat**
- **Completions**
- **Message**
- **Messages**

## Root Components

- **AddConnectionModal**
- **AddFilesPlaceholder**
- **AddServerModal**
- **ChangelogModal**
- **NotificationToast**
- **OnBoarding**

## Workspace Components

- **AccessControl**
- **AccessControlModal**
- **ActionsSelector**
- **AddContentMenu**
- **AddTextContentModal**
- **Capabilities**
- **CreateKnowledgeBase**
- **Files**
- **FiltersSelector**
- **ItemMenu**
- **Knowledge**
- **Knowledge**
- **KnowledgeBase**
- **ManifestModal**
- **ModelEditor**
- **ModelMenu**
- **Models**
- **PromptEditor**
- **PromptMenu**
- **Prompts**
- **Selector**
- **ToolMenu**
- **ToolkitEditor**
- **Tools**
- **ToolsSelector**
- **ValvesModal**
