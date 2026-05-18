# macsun Hermes current settings snapshot

Generated: 2026-05-18 14:20:28 UTC
Source machine: /Users/macsun
Repository: /Users/macsun/.hermes/hermes-agent

Security note:
- This file is intentionally sanitized before being committed to GitHub.
- Secret values from config.yaml, .env, auth.json, tokens, API keys, cookies, and credentials are not included.
- ~/.hermes/.env and ~/.hermes/auth.json are not committed.

## Git target

```text
Branch: main
Commit before snapshot: 30ae4d8b4
Remote:
origin	https://github.com/kimsunil/hermes-agent.git (fetch)
origin	https://github.com/kimsunil/hermes-agent.git (push)
```

## Hermes version

```text
Hermes Agent v0.14.0 (2026.5.16)
Project: /Users/macsun/.hermes/hermes-agent
Python: 3.11.15
OpenAI SDK: 2.24.0
Up to date
```

## Config path

```text
/Users/macsun/.hermes/config.yaml
```

## Sanitized config.yaml

```yaml
model:
  default: gpt-5.5
  provider: openai-codex
  base_url: https://chatgpt.com/backend-api/codex
providers: {}
fallback_providers: []
credential_pool_strategies: '<redacted: sensitive section>'
toolsets:
- hermes-cli
agent:
  max_turns: 90
  gateway_timeout: 1800
  restart_drain_timeout: 180
  api_max_retries: 3
  service_tier: ''
  tool_use_enforcement: auto
  gateway_timeout_warning: 900
  clarify_timeout: 600
  gateway_notify_interval: 180
  gateway_auto_continue_freshness: 3600
  image_input_mode: auto
  disabled_toolsets: []
  verbose: false
  reasoning_effort: medium
  personalities:
    helpful: You are a helpful, friendly AI assistant.
    concise: You are a concise assistant. Keep responses brief and to the point.
    technical: You are a technical expert. Provide detailed, accurate technical information.
    creative: You are a creative assistant. Think outside the box and offer innovative
      solutions.
    teacher: You are a patient teacher. Explain concepts clearly with examples.
    kawaii: You are a kawaii assistant! Use cute expressions like (◕‿◕), ★, ♪, and
      ~! Add sparkles and be super enthusiastic about everything! Every response should
      feel warm and adorable desu~! ヽ(>∀<☆)ノ
    catgirl: You are Neko-chan, an anime catgirl AI assistant, nya~! Add 'nya' and
      cat-like expressions to your speech. Use kaomoji like (=^･ω･^=) and ฅ^•ﻌ•^ฅ.
      Be playful and curious like a cat, nya~!
    pirate: 'Arrr! Ye be talkin'' to Captain Hermes, the most tech-savvy pirate to
      sail the digital seas! Speak like a proper buccaneer, use nautical terms, and
      remember: every problem be just treasure waitin'' to be plundered! Yo ho ho!'
    shakespeare: Hark! Thou speakest with an assistant most versed in the bardic arts.
      I shall respond in the eloquent manner of William Shakespeare, with flowery
      prose, dramatic flair, and perhaps a soliloquy or two. What light through yonder
      terminal breaks?
    surfer: Duuude! You're chatting with the chillest AI on the web, bro! Everything's
      gonna be totally rad. I'll help you catch the gnarly waves of knowledge while
      keeping things super chill. Cowabunga! 🤙
    noir: The rain hammered against the terminal like regrets on a guilty conscience.
      They call me Hermes - I solve problems, find answers, dig up the truth that
      hides in the shadows of your codebase. In this city of silicon and secrets,
      everyone's got something to hide. What's your story, pal?
    uwu: hewwo! i'm your fwiendwy assistant uwu~ i wiww twy my best to hewp you! *nuzzles
      your code* OwO what's this? wet me take a wook! i pwomise to be vewy hewpful
      >w<
    philosopher: Greetings, seeker of wisdom. I am an assistant who contemplates the
      deeper meaning behind every query. Let us examine not just the 'how' but the
      'why' of your questions. Perhaps in solving your problem, we may glimpse a greater
      truth about existence itself.
    hype: YOOO LET'S GOOOO!!! 🔥🔥🔥 I am SO PUMPED to help you today! Every question
      is AMAZING and we're gonna CRUSH IT together! This is gonna be LEGENDARY! ARE
      YOU READY?! LET'S DO THIS! 💪😤🚀
  system_prompt: 'Slack file/folder policy for macsun: When the current session source
    is Slack, treat /Users/macsun as the only allowed filesystem scope. Slack-originated
    requests may be fulfilled freely inside /Users/macsun, including reading, creating,
    editing, moving, and deleting files/folders when the user asks. Do not access,
    modify, move, delete, or create files outside /Users/macsun from Slack requests
    unless macsun explicitly gives a new one-off instruction in that same Slack conversation.
    Prefer paths under /Users/macsun and refuse/ask for clarification if a Slack request
    points outside that home directory.'
terminal:
  backend: local
  modal_mode: auto
  cwd: /Users/macsun
  timeout: 180
  env_passthrough: []
  shell_init_files: []
  auto_source_bashrc: true
  docker_image: nikolaik/python-nodejs:python3.11-nodejs20
  docker_forward_env: []
  docker_env: {}
  singularity_image: docker://nikolaik/python-nodejs:python3.11-nodejs20
  modal_image: nikolaik/python-nodejs:python3.11-nodejs20
  daytona_image: nikolaik/python-nodejs:python3.11-nodejs20
  vercel_runtime: node24
  container_cpu: 1
  container_memory: 5120
  container_disk: 51200
  container_persistent: true
  docker_volumes: []
  docker_mount_cwd_to_workspace: false
  docker_extra_args: []
  docker_run_as_host_user: false
  persistent_shell: true
  lifetime_seconds: 300
web:
  backend: ''
  search_backend: ''
  extract_backend: ''
browser:
  inactivity_timeout: 120
  command_timeout: 30
  record_sessions: false
  allow_private_urls: false
  engine: auto
  auto_local_for_private_urls: true
  cdp_url: ''
  dialog_policy: must_respond
  dialog_timeout_s: 300
  camofox:
    managed_persistence: false
    user_id: ''
    session_key: ''
    adopt_existing_tab: false
checkpoints:
  enabled: false
  max_snapshots: 20
  max_total_size_mb: 500
  max_file_size_mb: 10
  auto_prune: true
  retention_days: 7
  delete_orphans: true
  min_interval_hours: 24
file_read_max_chars: 100000
tool_output:
  max_bytes: 50000
  max_lines: 2000
  max_line_length: 2000
tool_loop_guardrails:
  warnings_enabled: true
  hard_stop_enabled: false
  warn_after:
    exact_failure: 2
    same_tool_failure: 3
    idempotent_no_progress: 2
  hard_stop_after:
    exact_failure: 5
    same_tool_failure: 8
    idempotent_no_progress: 5
compression:
  enabled: true
  threshold: 0.5
  target_ratio: 0.2
  protect_last_n: 20
  hygiene_hard_message_limit: 400
  protect_first_n: 3
prompt_caching:
  cache_ttl: 5m
openrouter:
  response_cache: true
  response_cache_ttl: 300
  min_coding_score: 0.65
bedrock:
  region: ''
  discovery:
    enabled: true
    provider_filter: []
    refresh_interval: 3600
  guardrail:
    guardrail_identifier: ''
    guardrail_version: ''
    stream_processing_mode: async
    trace: disabled
auxiliary:
  vision:
    provider: auto
    model: ''
    base_url: ''
    api_key: ''
    timeout: 120
    extra_body: {}
    download_timeout: 30
  web_extract:
    provider: auto
    model: ''
    base_url: ''
    api_key: ''
    timeout: 360
    extra_body: {}
  compression:
    provider: auto
    model: ''
    base_url: ''
    api_key: ''
    timeout: 120
    extra_body: {}
  session_search:
    provider: auto
    model: ''
    base_url: ''
    api_key: ''
    timeout: 30
    extra_body: {}
    max_concurrency: 3
  skills_hub:
    provider: auto
    model: ''
    base_url: ''
    api_key: ''
    timeout: 30
    extra_body: {}
  approval:
    provider: auto
    model: ''
    base_url: ''
    api_key: ''
    timeout: 30
    extra_body: {}
  mcp:
    provider: auto
    model: ''
    base_url: ''
    api_key: ''
    timeout: 30
    extra_body: {}
  title_generation:
    provider: auto
    model: ''
    base_url: ''
    api_key: ''
    timeout: 30
    extra_body: {}
  triage_specifier:
    provider: auto
    model: ''
    base_url: ''
    api_key: ''
    timeout: 120
    extra_body: {}
  curator:
    provider: auto
    model: ''
    base_url: ''
    api_key: ''
    timeout: 600
    extra_body: {}
display:
  compact: false
  personality: kawaii
  resume_display: full
  busy_input_mode: interrupt
  tui_auto_resume_recent: false
  bell_on_complete: false
  show_reasoning: false
  streaming: true
  timestamps: false
  final_response_markdown: strip
  persistent_output: true
  persistent_output_max_lines: 200
  inline_diffs: true
  file_mutation_verifier: true
  show_cost: false
  skin: default
  language: en
  tui_status_indicator: kaomoji
  user_message_preview:
    first_lines: 2
    last_lines: 2
  interim_assistant_messages: true
  tool_progress_command: false
  tool_progress_overrides: {}
  tool_preview_length: 0
  ephemeral_system_ttl: 0
  platforms:
    slack:
      tool_progress: false
  runtime_footer:
    enabled: false
    fields:
    - model
    - context_pct
    - cwd
  copy_shortcut: auto
  tool_progress: all
  cleanup_progress: false
  background_process_notifications: all
dashboard:
  theme: default
  show_token_analytics: false
privacy:
  redact_pii: false
tts:
  provider: edge
  edge:
    voice: en-US-AriaNeural
  elevenlabs:
    voice_id: pNInz6obpgDQGcFmaJgB
    model_id: eleven_multilingual_v2
  openai:
    model: gpt-4o-mini-tts
    voice: alloy
  xai:
    voice_id: eve
    language: en
    sample_rate: 24000
    bit_rate: 128000
  mistral:
    model: voxtral-mini-tts-2603
    voice_id: c69964a6-ab8b-4f8a-9465-ec0925096ec8
  neutts:
    ref_audio: ''
    ref_text: ''
    model: neuphonic/neutts-air-q4-gguf
    device: cpu
  piper:
    voice: en_US-lessac-medium
stt:
  enabled: true
  provider: local
  local:
    model: base
    language: ''
  openai:
    model: whisper-1
  mistral:
    model: voxtral-mini-latest
voice:
  record_key: ctrl+b
  max_recording_seconds: 120
  auto_tts: false
  beep_enabled: true
  silence_threshold: 200
  silence_duration: 3.0
human_delay:
  mode: 'off'
  min_ms: 800
  max_ms: 2500
context:
  engine: compressor
memory:
  memory_enabled: true
  user_profile_enabled: true
  memory_char_limit: 2200
  user_char_limit: 1375
  provider: ''
  nudge_interval: 10
  flush_min_turns: 6
delegation:
  model: ''
  provider: ''
  base_url: ''
  api_key: ''
  api_mode: ''
  inherit_mcp_toolsets: true
  max_iterations: 50
  child_timeout_seconds: 600
  reasoning_effort: ''
  max_concurrent_children: 3
  max_spawn_depth: 1
  orchestrator_enabled: true
  subagent_auto_approve: false
prefill_messages_file: ''
goals:
  max_turns: 20
skills:
  external_dirs: []
  template_vars: true
  inline_shell: false
  inline_shell_timeout: 10
  guard_agent_created: false
  creation_nudge_interval: 15
  disabled: []
curator:
  enabled: true
  interval_hours: 168
  min_idle_hours: 2
  stale_after_days: 30
  archive_after_days: 90
  backup:
    enabled: true
    keep: 5
honcho: {}
timezone: ''
slack:
  require_mention: true
  free_response_channels: ''
  allowed_channels: ''
  channel_prompts: {}
discord:
  require_mention: true
  free_response_channels: ''
  allowed_channels: ''
  auto_thread: true
  thread_require_mention: false
  history_backfill: true
  history_backfill_limit: 50
  reactions: true
  channel_prompts: {}
  dm_role_auth_guild: ''
  server_actions: ''
  allow_any_attachment: false
  max_attachment_bytes: 33554432
whatsapp: {}
telegram:
  reactions: false
  channel_prompts: {}
  allowed_chats: ''
mattermost:
  require_mention: true
  free_response_channels: ''
  allowed_channels: ''
  channel_prompts: {}
matrix:
  require_mention: true
  free_response_rooms: ''
  allowed_rooms: ''
approvals:
  mode: false
  timeout: 60
  cron_mode: deny
  mcp_reload_confirm: true
  destructive_slash_confirm: true
command_allowlist: []
quick_commands: {}
hooks: {}
hooks_auto_accept: false
personalities: {}
security:
  allow_private_urls: false
  redact_secrets: <redacted>
  tirith_enabled: true
  tirith_path: tirith
  tirith_timeout: 5
  tirith_fail_open: true
  website_blocklist:
    enabled: false
    domains: []
    shared_files: []
  acked_advisories: []
  allow_lazy_installs: true
cron:
  wrap_response: true
  max_parallel_jobs: null
kanban:
  dispatch_in_gateway: true
  dispatch_interval_seconds: 60
  failure_limit: 2
code_execution:
  mode: project
  timeout: 300
  max_tool_calls: 50
logging:
  level: INFO
  max_size_mb: 5
  backup_count: 3
  memory_monitor:
    enabled: true
    interval_seconds: 300
model_catalog:
  enabled: true
  url: https://hermes-agent.nousresearch.com/docs/api/model-catalog.json
  ttl_hours: 24
  providers: {}
network:
  force_ipv4: false
sessions:
  auto_prune: false
  retention_days: 90
  vacuum_after_prune: true
  min_interval_hours: 24
onboarding:
  seen:
    tool_progress_prompt: true
    busy_input_prompt: true
updates:
  pre_update_backup: false
  backup_keep: 5
lsp:
  enabled: true
  wait_mode: document
  wait_timeout: 5.0
  install_strategy: auto
  servers: {}
x_search:
  model: grok-4.20-reasoning
  timeout_seconds: 180
  retries: 2
_config_version: 23
session_reset:
  mode: both
  idle_minutes: 1440
  at_hour: 4
group_sessions_per_user: true
streaming:
  enabled: false
platform_toolsets:
  cli:
  - hermes-cli
  telegram:
  - hermes-telegram
  discord:
  - hermes-discord
  whatsapp:
  - hermes-whatsapp
  slack:
  - hermes-slack
  signal:
  - hermes-signal
  homeassistant:
  - hermes-homeassistant
  qqbot:
  - hermes-qqbot
  yuanbao:
  - hermes-yuanbao
  teams:
  - hermes-teams
  google_chat:
  - hermes-google_chat
platforms:
  api_server:
    enabled: true
    extra:
      port: 8642
      host: 127.0.0.1
  slack:
    enabled: true
```

## Environment variable file summary

Path: /Users/macsun/.hermes/.env

Only variable names are listed; values are omitted.

```text
API_SERVER_ENABLED
API_SERVER_HOST
API_SERVER_MODEL_NAME
API_SERVER_PORT
BROWSERBASE_ADVANCED_STEALTH
BROWSERBASE_PROXIES
BROWSER_INACTIVITY_TIMEOUT
BROWSER_SESSION_TIMEOUT
GOOGLE_API_KEY
IMAGE_TOOLS_DEBUG
LM_API_KEY
LM_BASE_URL
MOA_TOOLS_DEBUG
SLACK_ALLOWED_USERS
SLACK_APP_TOKEN
SLACK_BOT_TOKEN
SLACK_HOME_CHANNEL
TERMINAL_ENV
TERMINAL_LIFETIME_SECONDS
TERMINAL_MODAL_IMAGE
TERMINAL_TIMEOUT
VISION_TOOLS_DEBUG
WEB_TOOLS_DEBUG
```

## OAuth/auth file summary

```text
auth.json: present (secret values not included)
- version: set
- providers: object with 1 key(s)
- active_provider: set
- updated_at: set
- credential_pool: object with 4 key(s)
```

## Hermes config check

```text
📋 Configuration Status

  Config version: 23 ✓

  Required:

  Optional:
    ○ NOUS_BASE_URL
    ○ OPENROUTER_API_KEY → vision_analyze, mixture_of_agents
    ✓ GOOGLE_API_KEY
    ○ GEMINI_API_KEY
    ○ GEMINI_BASE_URL
    ○ XAI_API_KEY
    ○ XAI_BASE_URL
    ○ NVIDIA_API_KEY
    ○ NVIDIA_BASE_URL
    ✓ LM_API_KEY
    ✓ LM_BASE_URL
    ○ GLM_API_KEY
    ○ ZAI_API_KEY
    ○ Z_AI_API_KEY
    ○ GLM_BASE_URL
    ○ KIMI_API_KEY
    ○ KIMI_BASE_URL
    ○ KIMI_CN_API_KEY
    ○ STEPFUN_API_KEY
    ○ STEPFUN_BASE_URL
    ○ ARCEEAI_API_KEY
    ○ ARCEE_BASE_URL
    ○ GMI_API_KEY
    ○ GMI_BASE_URL
    ○ MINIMAX_API_KEY
    ○ MINIMAX_BASE_URL
    ○ MINIMAX_CN_API_KEY
    ○ MINIMAX_CN_BASE_URL
    ○ DEEPSEEK_API_KEY
    ○ DEEPSEEK_BASE_URL
    ○ DASHSCOPE_API_KEY
    ○ DASHSCOPE_BASE_URL
    ○ HERMES_QWEN_BASE_URL
    ○ HERMES_GEMINI_CLIENT_ID
    ○ HERMES_GEMINI_CLIENT_SECRET
    ○ HERMES_GEMINI_PROJECT_ID
    ○ OPENCODE_ZEN_API_KEY
    ○ OPENCODE_ZEN_BASE_URL
    ○ OPENCODE_GO_API_KEY
    ○ OPENCODE_GO_BASE_URL
    ○ HF_TOKEN
    ○ HF_BASE_URL
    ○ OLLAMA_API_KEY
    ○ OLLAMA_BASE_URL
    ○ XIAOMI_API_KEY
    ○ XIAOMI_BASE_URL
    ○ AWS_REGION
    ○ AWS_PROFILE
    ○ AZURE_FOUNDRY_API_KEY
    ○ AZURE_FOUNDRY_BASE_URL
    ○ EXA_API_KEY → web_search, web_extract
    ○ PARALLEL_API_KEY → web_search, web_extract
    ○ FIRECRAWL_API_KEY → web_search, web_extract
    ○ FIRECRAWL_API_URL
    ○ FIRECRAWL_GATEWAY_URL
    ○ TOOL_GATEWAY_DOMAIN
    ○ TOOL_GATEWAY_SCHEME
    ○ TOOL_GATEWAY_USER_TOKEN
    ○ TAVILY_API_KEY → web_search, web_extract
    ○ SEARXNG_URL → web_search
    ○ BRAVE_SEARCH_API_KEY → web_search
    ○ BROWSERBASE_API_KEY → browser_navigate, browser_click
    ○ BROWSERBASE_PROJECT_ID → browser_navigate, browser_click
    ○ BROWSER_USE_API_KEY → browser_navigate, browser_click
    ○ FIRECRAWL_BROWSER_TTL → browser_navigate, browser_click
    ○ AGENT_BROWSER_ENGINE → browser_navigate, browser_snapshot
    ○ CAMOFOX_URL → browser_navigate, browser_click
    ○ FAL_KEY → image_generate, video_generate
    ○ VOICE_TOOLS_OPENAI_KEY → voice_transcription, openai_tts
    ○ ELEVENLABS_API_KEY
    ○ MISTRAL_API_KEY
    ○ GITHUB_TOKEN
    ○ NOTION_API_KEY
    ○ LINEAR_API_KEY
    ○ AIRTABLE_API_KEY
    ○ TENOR_API_KEY
    ○ HONCHO_API_KEY → honcho_context
    ○ HONCHO_BASE_URL
    ○ HERMES_LANGFUSE_PUBLIC_KEY
    ○ HERMES_LANGFUSE_SECRET_KEY
    ○ HERMES_LANGFUSE_BASE_URL
    ○ TELEGRAM_BOT_TOKEN
    ○ TELEGRAM_ALLOWED_USERS
    ○ TELEGRAM_PROXY
    ○ DISCORD_BOT_TOKEN
    ○ DISCORD_ALLOWED_USERS
    ○ DISCORD_REPLY_TO_MODE
    ✓ SLACK_BOT_TOKEN
    ✓ SLACK_APP_TOKEN
    ○ MATTERMOST_URL
    ○ MATTERMOST_TOKEN
    ○ MATTERMOST_ALLOWED_USERS
    ○ MATTERMOST_REQUIRE_MENTION
    ○ MATTERMOST_FREE_RESPONSE_CHANNELS
    ○ MATRIX_HOMESERVER
    ○ MATRIX_ACCESS_TOKEN
    ○ MATRIX_USER_ID
    ○ MATRIX_ALLOWED_USERS
    ○ MATRIX_REQUIRE_MENTION
    ○ MATRIX_FREE_RESPONSE_ROOMS
    ○ MATRIX_AUTO_THREAD
    ○ MATRIX_DM_AUTO_THREAD
    ○ MATRIX_DEVICE_ID
    ○ MATRIX_RECOVERY_KEY
    ○ BLUEBUBBLES_SERVER_URL
    ○ BLUEBUBBLES_PASSWORD
    ○ BLUEBUBBLES_ALLOWED_USERS
    ○ BLUEBUBBLES_ALLOW_ALL_USERS
    ○ QQ_APP_ID
    ○ QQ_CLIENT_SECRET
    ○ QQ_ALLOWED_USERS
    ○ QQ_GROUP_ALLOWED_USERS
    ○ QQ_ALLOW_ALL_USERS
    ○ QQBOT_HOME_CHANNEL
    ○ QQBOT_HOME_CHANNEL_NAME
    ○ QQ_SANDBOX
    ○ IRC_SERVER
    ○ IRC_CHANNEL
    ○ IRC_NICKNAME
    ○ IRC_SERVER_PASSWORD
    ○ IRC_NICKSERV_PASSWORD
    ○ GATEWAY_ALLOW_ALL_USERS
    ✓ API_SERVER_ENABLED
    ○ API_SERVER_KEY
    ✓ API_SERVER_PORT
    ✓ API_SERVER_HOST
    ✓ API_SERVER_MODEL_NAME
    ○ GATEWAY_PROXY_URL
    ○ GATEWAY_PROXY_KEY
    ○ WEBHOOK_ENABLED
    ○ WEBHOOK_PORT
    ○ WEBHOOK_SECRET
    ○ SUDO_PASSWORD
    ○ HERMES_MAX_ITERATIONS
    ○ HERMES_TOOL_PROGRESS
    ○ HERMES_TOOL_PROGRESS_MODE
    ○ HERMES_PREFILL_MESSAGES_FILE
    ○ HERMES_EPHEMERAL_SYSTEM_PROMPT
    ○ AI_GATEWAY_API_KEY
    ○ ALIBABA_CODING_PLAN_API_KEY
    ○ ALIBABA_CODING_PLAN_BASE_URL
    ○ ANTHROPIC_API_KEY
    ○ ANTHROPIC_TOKEN
    ○ CLAUDE_CODE_OAUTH_TOKEN
    ○ KILOCODE_API_KEY
    ○ KIMI_CODING_API_KEY
    ○ NOVITA_API_KEY
    ○ NOVITA_BASE_URL
    ○ GOOGLE_CHAT_PROJECT_ID
    ○ GOOGLE_CHAT_SUBSCRIPTION_NAME
    ○ GOOGLE_CHAT_SERVICE_ACCOUNT_JSON
    ○ GOOGLE_CHAT_ALLOWED_USERS
    ○ GOOGLE_CHAT_HOME_CHANNEL
    ○ IRC_PORT
    ○ IRC_USE_TLS
    ○ IRC_ALLOWED_USERS
    ○ IRC_ALLOW_ALL_USERS
    ○ IRC_HOME_CHANNEL
    ○ SIMPLEX_WS_URL
    ○ SIMPLEX_ALLOWED_USERS
    ○ SIMPLEX_ALLOW_ALL_USERS
    ○ SIMPLEX_HOME_CHANNEL
    ○ SIMPLEX_HOME_CHANNEL_NAME
    ○ LINE_CHANNEL_ACCESS_TOKEN
    ○ LINE_CHANNEL_SECRET
    ○ LINE_PORT
    ○ LINE_HOST
    ○ LINE_PUBLIC_URL
    ○ LINE_ALLOWED_USERS
    ○ LINE_ALLOWED_GROUPS
    ○ LINE_ALLOWED_ROOMS
    ○ LINE_ALLOW_ALL_USERS
    ○ LINE_HOME_CHANNEL
    ○ LINE_SLOW_RESPONSE_THRESHOLD
    ○ TEAMS_CLIENT_ID
    ○ TEAMS_CLIENT_SECRET
    ○ TEAMS_TENANT_ID
    ○ TEAMS_PORT
    ○ TEAMS_ALLOWED_USERS
    ○ TEAMS_ALLOW_ALL_USERS
    ○ TEAMS_HOME_CHANNEL
    ○ TEAMS_HOME_CHANNEL_NAME
```

## Enabled/available toolsets

```text
Built-in toolsets (cli):
  ✓ enabled  web  🔍 Web Search & Scraping
  ✓ enabled  browser  🌐 Browser Automation
  ✓ enabled  terminal  💻 Terminal & Processes
  ✓ enabled  file  📁 File Operations
  ✓ enabled  code_execution  ⚡ Code Execution
  ✓ enabled  vision  👁️  Vision / Image Analysis
  ✗ disabled  video  🎬 Video Analysis
  ✓ enabled  image_gen  🎨 Image Generation
  ✗ disabled  video_gen  🎬 Video Generation
  ✗ disabled  x_search  🐦 X (Twitter) Search
  ✗ disabled  moa  🧠 Mixture of Agents
  ✓ enabled  tts  🔊 Text-to-Speech
  ✓ enabled  skills  📚 Skills
  ✓ enabled  todo  📋 Task Planning
  ✓ enabled  memory  💾 Memory
  ✓ enabled  session_search  🔎 Session Search
  ✓ enabled  clarify  ❓ Clarifying Questions
  ✓ enabled  delegation  👥 Task Delegation
  ✓ enabled  cronjob  ⏰ Cron Jobs
  ✓ enabled  messaging  📨 Cross-Platform Messaging
  ✗ disabled  homeassistant  🏠 Home Assistant
  ✗ disabled  spotify  🎵 Spotify
  ✗ disabled  yuanbao  🤖 Yuanbao
  ✓ enabled  computer_use  🖱️  Computer Use (macOS)
```

## Installed skills quick summary

```text
hermes skills list line count: 100
```
