# Orchestrators

Многоагентные системы — дирижируют несколькими агентами одновременно (например, запускают параллельных воркеров на разные куски проекта). Бери оркестратор, когда одной головы мало и нужно раздать работу.

## Ресурсы

### [claude-code-orchestrator-kit](https://github.com/maslennikov-ig/claude-code-orchestrator-kit)

**Что даёт:** 49 агентов + 42 собственных скилла + SpecKit (11-шаговый workflow "Claude = оркестратор, агенты = воркеры"); агенты реально читают скиллы как source of truth, а не дублируют логику
**Когда брать:** стек близок к Node.js/TypeScript/Supabase, либо нужна эталонная архитектура многоагентной системы для изучения (health-домен и SpecKit переносимы, development-домен заточен под LMS-проект автора)
**Для чего лучше:** backend (TypeScript/Node.js/Supabase), fullstack
**Установка:** `git clone https://github.com/maslennikov-ig/claude-code-orchestrator-kit`
**Автор:** [@maslennikov-ig](https://github.com/maslennikov-ig)

### [claude-code-orchestrator-python](https://github.com/Baktiyar88/claude-code-orchestrator-python)

**Что даёт:** готовая Claude Code среда — 48 агентов + 54+ собственных скилла (django-patterns, django-tdd, django-security, code-review); агенты при запуске читают соответствующие SKILL.md как source of truth
**Когда брать:** стек строго Django + DRF + PostgreSQL + Celery; готов заполнить CLAUDE.md-шаблон под свой проект; принимаешь что репо свежее (апрель 2026) и ещё не обкатано сообществом
**Для чего лучше:** backend (Python/Django)
**Установка:** `git clone https://github.com/Baktiyar88/claude-code-orchestrator-python && bash install.sh`
**Автор:** [@Baktiyar88](https://github.com/Baktiyar88)

---

## Шаблон карточки (для новых ресурсов)

```markdown
### [название](https://github.com/user/repo)

**Что даёт:** одно предложение про полезность
**Когда брать:** одно предложение про use-case
**Для чего лучше:** универсал / backend / frontend / mobile / data
**Установка:** команда или ссылка на инструкцию
**Автор:** [@username](https://github.com/username)
```

См. также [CONTRIBUTING.md](../CONTRIBUTING.md).