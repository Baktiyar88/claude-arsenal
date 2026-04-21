# 📚 Browse — ещё больше ресурсов

> ⚠️ **Эти репо я не проверял детально.** Собраны из поиска GitHub по популярности (звёзды, активность, упоминания в awesome-lists). Перед использованием открой репо, прочитай README, пролистай код. Не копируй слепо.

**Чем отличается от основных папок?** В папках [`frameworks/`](../frameworks/), [`orchestrators/`](../orchestrators/), [`tools/`](../tools/), [`agents-skills/`](../agents-skills/), [`automation/`](../automation/), [`docs/`](../docs/) лежат **проверенные** ресурсы с разбором "что даёт / когда брать / для чего лучше". Здесь — просто список популярного, для самостоятельного изучения.

**Всё что ниже — бесплатное** (локальные инструменты без подписок). Требуется только твой Claude API / Claude Pro.

---

## 📦 Frameworks (методологии "всё-в-одном")

- [affaan-m/everything-claude-code](https://github.com/affaan-m/everything-claude-code) — 163k ⭐ — 48 агентов + 183 скилла + 34 ruleset + 20 хуков + 14 MCP; мультиплатформа (Claude / Cursor / Codex / OpenCode)
- [gsd-build/get-shit-done](https://github.com/gsd-build/get-shit-done) — 55.7k ⭐ — мета-промптинг, 5-фазный цикл (init → discuss → plan → execute → verify), решает "context rot"
- [shanraisshan/claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice) — 47.1k ⭐ — гид по структуре CLAUDE.md, ленивая загрузка через `.claude/rules/*.md`, монорепо-паттерны
- [wshobson/agents](https://github.com/wshobson/agents) — 34k ⭐ — 184 агента + 150 скиллов + 78 плагинов, три-тирный выбор моделей (Opus/Sonnet/Haiku)

## 🎭 Orchestrators (команды агентов)

- [ruvnet/ruflo](https://github.com/ruvnet/ruflo) — 32.7k ⭐ — оркестрация роёв агентов + RAG + MCP, nativ интеграция с Claude Code и Codex
- [Yeachan-Heo/oh-my-claudecode](https://github.com/Yeachan-Heo/oh-my-claudecode) — 30.5k ⭐ — teams-first, 19 агентов, tmux-воркеры, real-time HUD с метриками
- [21st-dev/1code](https://github.com/21st-dev/1code) — 5.5k ⭐ — визуальный UI-оркестратор, git worktree на каждую сессию, live diff preview
- [stellarlinkco/myclaude](https://github.com/stellarlinkco/myclaude) — 2.6k ⭐ — роутинг задач между Claude / Codex / Gemini / OpenCode через единый интерфейс

## 🧑‍🔧 Agents & Skills (специалисты)

- [sickn33/antigravity-awesome-skills](https://github.com/sickn33/antigravity-awesome-skills) — 34.4k ⭐ — 1431+ skill playbook, npx-установка, кросс-платформа
- [VoltAgent/awesome-claude-code-subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) — 17.9k ⭐ — 130+ субагентов по 10 категориям (языки, инфра, QA, ML, meta-orchestration)
- [rohitg00/awesome-claude-code-toolkit](https://github.com/rohitg00/awesome-claude-code-toolkit) — 1.4k ⭐ — 135 агентов + 35 скиллов + 42 команды + 176+ плагинов — всё одним пакетом

## 🛠 Tools & MCP Servers (локальные, без внешних сервисов)

- [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) — 84.2k ⭐ — **официальный Anthropic** MCP: Filesystem / Git / Memory / Sequential Thinking / Fetch / Time
- [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) — 36.6k ⭐ — **официальный Google** — контроль локального Chrome, отладка сети, Lighthouse, профилирование
- [github/github-mcp-server](https://github.com/github/github-mcp-server) — 29.1k ⭐ — **официальный GitHub** MCP: репо, issues, PR, Actions через Claude (нужен бесплатный GitHub PAT)
- [wonderwhy-er/DesktopCommanderMCP](https://github.com/wonderwhy-er/DesktopCommanderMCP) — 5.9k ⭐ — полный системный доступ (терминал, файлы Excel/PDF/DOCX, Python/Node/R в памяти, SSH)

## 🪝 Hooks & Automation

- [diet103/claude-code-infrastructure-showcase](https://github.com/diet103/claude-code-infrastructure-showcase) — 9.5k ⭐ — 6 месяцев production опыта: авто-активация скиллов через UserPromptSubmit, TypeScript-валидация, авто-резолв билдов
- [parcadei/Continuous-Claude-v3](https://github.com/parcadei/Continuous-Claude-v3) — 3.7k ⭐ — 95% экономии токенов, память между сессиями на PostgreSQL+pgvector, 30 хуков, 109 скиллов
- [disler/claude-code-hooks-mastery](https://github.com/disler/claude-code-hooks-mastery) — 3.5k ⭐ — курс по всем 13 типам хуков — единственный полный учебник
- [nizos/tdd-guard](https://github.com/nizos/tdd-guard) — 2k ⭐ — хук принуждает к TDD, блокирует реализацию без тестов (Vitest / Jest / pytest / PHPUnit / Go / Rust / RSpec)
- [rohitg00/pro-workflow](https://github.com/rohitg00/pro-workflow) — 2k ⭐ — самокорректирующаяся память: сохраняет твои исправления в SQLite, автоматически применяет их в новых сессиях

## 📄 Templates & Official

- [anthropics/anthropic-quickstarts](https://github.com/anthropics/anthropic-quickstarts) — 16.2k ⭐ — **официальные шаблоны Anthropic**: Customer Support Agent, Financial Data Analyst, Computer Use Demo, Autonomous Coding Agent
- [davepoon/buildwithclaude](https://github.com/davepoon/buildwithclaude) — 2.8k ⭐ — агрегатор 20k+ community-плагинов + веб-интерфейс buildwithclaude.com с поиском и one-click установкой

## 📋 Awesome Lists (каталоги каталогов)

- [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) — 85.3k ⭐ — **главный каталог MCP-серверов** (>5900 коммитов), тысячи серверов по категориям
- [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) — 40.1k ⭐ — **главный awesome-list Claude Code** (скиллы/хуки/команды/оркестраторы/плагины/альтернативные клиенты)
- [travisvn/awesome-claude-skills](https://github.com/travisvn/awesome-claude-skills) — 11.6k ⭐ — awesome-list скиллов: официальные Anthropic + лучшие community (включая obra/superpowers)

---

## Как ресурс переезжает отсюда в основные папки?

Если после изучения репо оказывается реально полезным — переноси его в соответствующую папку ([frameworks/](../frameworks/), [orchestrators/](../orchestrators/) и т.д.) и пиши полноценную карточку "что даёт / когда брать / для чего лучше / установка / автор".

Как это делается — см. [CONTRIBUTING.md](../CONTRIBUTING.md).
