# 🧰 claude-arsenal

Сборник всего, что делает [Claude Code](https://claude.com/claude-code) сильнее. Один клик — одна понятная польза.

Это awesome-list: только ссылки на публичные репо + краткие описания "что даёт / когда брать / для чего лучше". Код внутрь не копируем, лицензии оригиналов не нарушаем.

---

## 🎯 Что тебе нужно?

### «Хочу универсал с хорошей памятью и контекстом»
→ [superpowers](frameworks/README.md) — полный workflow разработки, понимает контекст любого стэка (бэк + фронт)

### «Хочу чтобы Claude быстро разбирался в большом проекте»
→ [graphify](tools/README.md) — строит "карту связей" твоего кода и документации, Claude через неё находит нужное мгновенно вместо чтения всего подряд

### «Хочу команду Claude-агентов под мой Node.js/TypeScript/Supabase бэк»
→ [claude-code-orchestrator-kit](orchestrators/README.md) — готовый набор из 49 специализированных агентов (поиск багов, безопасность, код-ревью, архитектор) работающих одновременно под управлением главного Claude

### «Хочу команду Claude-агентов под мой Django/DRF/PostgreSQL бэк»
→ [claude-code-orchestrator-python](orchestrators/README.md) — то же самое, но под Django-стэк (48 агентов + 54+ скиллов)

### «Хочу точечного специалиста (planner, reviewer, architect)»
→ [agents-skills/](agents-skills/README.md)

### «Хочу готовые хуки и шаблоны CLAUDE.md»
→ [automation/](automation/README.md)

### «Хочу гайды и шпаргалки»
→ [docs/](docs/README.md)

---

## 📁 Все папки

| Папка | Что там | Примеры |
|---|---|---|
| [frameworks/](frameworks/) | Методологии "всё-в-одном" | superpowers |
| [orchestrators/](orchestrators/) | Команды агентов (многоагентные системы) | claude-code-orchestrator-kit, claude-code-orchestrator-python |
| [agents-skills/](agents-skills/) | Отдельные агенты и скиллы | _пусто_ |
| [tools/](tools/) | MCP серверы, утилиты | graphify |
| [automation/](automation/) | Хуки, промпты, шаблоны CLAUDE.md | _пусто_ |
| [docs/](docs/) | Гайды и шпаргалки | _пусто_ |

---

## 🤝 Добавить свой ресурс

1. Читай короткий [CONTRIBUTING.md](CONTRIBUTING.md).
2. Открой [issue по шаблону](../../issues/new/choose) (30 секунд) **или** сделай Pull Request с новой карточкой в нужной папке.

**Правила:** только публичные репо с открытой лицензией (MIT, Apache, GPL и т.п.). Атрибуция автора обязательна.

---

## 📜 Лицензия

[MIT](LICENSE) — для самого этого каталога. Все перечисленные ресурсы остаются под лицензиями их авторов.
