# claude-arsenal — Implementation Plan (Scaffolding)

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build out the initial scaffolding of claude-arsenal (folders, READMEs, LICENSE, CONTRIBUTING, issue template, .gitignore) per the approved spec, then push to `origin/main`.

**Architecture:** Awesome-list style public repo. 6 top-level folders each with their own README using a unified resource card format. Root README uses "what do you need?" navigation. No code, no CI — pure markdown + one YAML issue template.

**Tech Stack:** Markdown, GitHub Flavored Markdown, YAML (for GitHub issue forms), git.

**Source spec:** `docs/superpowers/specs/2026-04-21-claude-arsenal-structure-design.md`

**Current repo state:** Initialized, remote `origin` points to `https://github.com/Baktiyar88/claude-arsenal.git`, 1 commit exists (spec). No files yet besides the spec.

**Verification approach:** Since this is a docs-only repo, "tests" are: (a) `ls` to confirm file structure, (b) read back written content, (c) `git log` to confirm commits, (d) final visual check on GitHub after push.

---

## File Structure

Files created by this plan, grouped by commit:

| Commit | File | Purpose |
|---|---|---|
| 1 | `.gitignore` | Exclude OS/editor junk from repo |
| 1 | `LICENSE` | MIT license |
| 2 | `frameworks/README.md` | Category page with superpowers card |
| 2 | `orchestrators/README.md` | Category page with empty-state + card template |
| 2 | `agents-skills/README.md` | Category page with empty-state + card template |
| 2 | `tools/README.md` | Category page with graphify card |
| 2 | `automation/README.md` | Category page with empty-state + card template |
| 2 | `docs/README.md` | Docs index |
| 3 | `README.md` | Root navigation hub ("what do you need?") |
| 4 | `CONTRIBUTING.md` | How to add a resource |
| 4 | `.github/ISSUE_TEMPLATE/add-resource.yml` | Issue form for non-PR contributors |

Four logical commits. Final step pushes to `origin/main`.

---

## Task 1: Add LICENSE and .gitignore

**Files:**
- Create: `LICENSE`
- Create: `.gitignore`

- [ ] **Step 1: Write `.gitignore`**

Create `C:\Users\Bokti\Desktop\claude-arsenal\.gitignore`:

```
# OS
.DS_Store
Thumbs.db
desktop.ini

# Editors
.vscode/
.idea/
*.swp
*.swo
*~

# Temp files
*.tmp
*.log
```

- [ ] **Step 2: Write `LICENSE`**

Create `C:\Users\Bokti\Desktop\claude-arsenal\LICENSE` with the standard MIT license, `{{year}}` = `2026`, `{{holder}}` = `Baktiyar88`:

```
MIT License

Copyright (c) 2026 Baktiyar88

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

- [ ] **Step 3: Verify files exist**

Run:
```bash
ls -la /c/Users/Bokti/Desktop/claude-arsenal/.gitignore /c/Users/Bokti/Desktop/claude-arsenal/LICENSE
```
Expected: both files listed, non-zero size.

- [ ] **Step 4: Commit**

```bash
cd /c/Users/Bokti/Desktop/claude-arsenal
git add .gitignore LICENSE
git commit -m "chore: add MIT LICENSE and .gitignore"
```

Expected: commit succeeds, `git log` shows 2 commits total.

---

## Task 2: Scaffold 6 category README files

**Files:**
- Create: `frameworks/README.md` (with superpowers card)
- Create: `orchestrators/README.md` (empty-state + template)
- Create: `agents-skills/README.md` (empty-state + template)
- Create: `tools/README.md` (with graphify card)
- Create: `automation/README.md` (empty-state + template)
- Create: `docs/README.md` (docs index)

- [ ] **Step 1: Write `frameworks/README.md`**

Create `C:\Users\Bokti\Desktop\claude-arsenal\frameworks\README.md`:

````markdown
# Frameworks

Целостные методологии "всё-в-одном" — обычно объединяют сразу skills, agents, hooks и commands в один пакет. Бери фреймворк, если хочешь отстроенный workflow и не хочешь собирать стек самостоятельно.

## Ресурсы

### [superpowers](https://github.com/obra/superpowers)

**Что даёт:** полный workflow разработки — брейншторм, планирование, TDD, код-ревью, дебаг в виде автоматически применяющихся скиллов
**Когда брать:** если хочешь отстроенный процесс, а не собирать всё с нуля
**Для чего лучше:** универсал (бэк + фронт, любой стэк)
**Установка:** `git clone https://github.com/obra/superpowers ~/.claude/plugins/superpowers`
**Автор:** [@obra](https://github.com/obra)

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
````

- [ ] **Step 2: Write `orchestrators/README.md`**

Create `C:\Users\Bokti\Desktop\claude-arsenal\orchestrators\README.md`:

````markdown
# Orchestrators

Многоагентные системы — дирижируют несколькими агентами одновременно (например, запускают параллельных воркеров на разные куски проекта). Бери оркестратор, когда одной головы мало и нужно раздать работу.

## Ресурсы

_Пока пусто. Добавь первый ресурс через PR или [issue](../../issues/new/choose)._

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
````

- [ ] **Step 3: Write `agents-skills/README.md`**

Create `C:\Users\Bokti\Desktop\claude-arsenal\agents-skills\README.md`:

````markdown
# Agents & Skills

Отдельные, самодостаточные агенты или скиллы — один инструмент, одна задача. Planner, code-reviewer, architect, security-reviewer и подобные. Бери сюда, если нужен точечный специалист, а не весь фреймворк.

## Ресурсы

_Пока пусто. Добавь первый ресурс через PR или [issue](../../issues/new/choose)._

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
````

- [ ] **Step 4: Write `tools/README.md`**

Create `C:\Users\Bokti\Desktop\claude-arsenal\tools\README.md`:

````markdown
# Tools

MCP-серверы, CLI-утилиты, внешние инструменты, которые требуют установки как отдельный сервис или пакет. Они расширяют capabilities Claude через Model Context Protocol или интеграции.

## Ресурсы

### [graphify](https://github.com/safishamsi/graphify)

**Что даёт:** превращает папку с кодом в queryable knowledge graph — AST анализ 25+ языков + MCP сервер + семантический поиск
**Когда брать:** когда хочешь чтобы Claude понимал связи и структуру в большой кодовой базе
**Для чего лучше:** универсал (особенно полезно на больших/сложных проектах и research по чужому коду)
**Установка:** см. инструкцию в репо (Python + MCP)
**Автор:** [@safishamsi](https://github.com/safishamsi)

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
````

- [ ] **Step 5: Write `automation/README.md`**

Create `C:\Users\Bokti\Desktop\claude-arsenal\automation\README.md`:

````markdown
# Automation

Хуки settings.json (PreToolUse, PostToolUse, Stop), шаблоны CLAUDE.md, заготовки промптов, преднастроенные permissions. Конфиги и шаблоны, а не исполняемый код.

## Ресурсы

_Пока пусто. Добавь первый ресурс через PR или [issue](../../issues/new/choose)._

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
````

- [ ] **Step 6: Write `docs/README.md`**

Create `C:\Users\Bokti\Desktop\claude-arsenal\docs\README.md`:

````markdown
# Docs

Гайды, шпаргалки, сравнения, заметки. Всё что читается как текст, а не исполняется.

## Внутренние документы

- [superpowers/specs/](superpowers/specs/) — спеки этого репо (design docs)
- [superpowers/plans/](superpowers/plans/) — implementation plans этого репо

## Гайды и шпаргалки

_Пока пусто. Добавь первый гайд через PR или [issue](../../issues/new/choose)._

---

## Шаблон карточки (если ссылаешься на внешний гайд)

```markdown
### [название гайда](URL)

**Что даёт:** одно предложение про пользу
**Когда читать:** одно предложение про use-case
**Для чего лучше:** универсал / backend / frontend / mobile / data
**Автор:** [@username](https://github.com/username)
```

См. также [CONTRIBUTING.md](../CONTRIBUTING.md).
````

- [ ] **Step 7: Verify all 6 READMEs exist**

Run:
```bash
ls /c/Users/Bokti/Desktop/claude-arsenal/frameworks/README.md \
   /c/Users/Bokti/Desktop/claude-arsenal/orchestrators/README.md \
   /c/Users/Bokti/Desktop/claude-arsenal/agents-skills/README.md \
   /c/Users/Bokti/Desktop/claude-arsenal/tools/README.md \
   /c/Users/Bokti/Desktop/claude-arsenal/automation/README.md \
   /c/Users/Bokti/Desktop/claude-arsenal/docs/README.md
```
Expected: all 6 files listed, no errors.

- [ ] **Step 8: Commit**

```bash
cd /c/Users/Bokti/Desktop/claude-arsenal
git add frameworks/README.md orchestrators/README.md agents-skills/README.md tools/README.md automation/README.md docs/README.md
git commit -m "feat: add 6 category READMEs with initial resources (superpowers, graphify)"
```

Expected: commit succeeds, 6 files added, `git log` shows 3 commits total.

---

## Task 3: Write root `README.md`

**Files:**
- Create: `README.md`

- [ ] **Step 1: Write root `README.md`**

Create `C:\Users\Bokti\Desktop\claude-arsenal\README.md`:

````markdown
# 🧰 claude-arsenal

Сборник всего, что делает [Claude Code](https://claude.com/claude-code) сильнее. Один клик — одна понятная польза.

Это awesome-list: только ссылки на публичные репо + краткие описания "что даёт / когда брать / для чего лучше". Код внутрь не копируем, лицензии оригиналов не нарушаем.

---

## 🎯 Что тебе нужно?

### «Хочу универсал с хорошей памятью и контекстом»
→ [superpowers](frameworks/README.md#superpowersgithubcomobrasuperpowers) — полный workflow разработки, понимает контекст любого стэка (бэк + фронт)

### «Хочу превратить кодовую базу в граф знаний»
→ [graphify](tools/README.md#graphifygithubcomsafishamsigraphify) — AST анализ 25+ языков + MCP + семантический поиск

### «Хочу оркестратор для бэкенда / фронтенда»
→ [orchestrators/](orchestrators/README.md) — многоагентные системы (пока пусто, добавляй!)

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
| [orchestrators/](orchestrators/) | Многоагентные системы | _пусто_ |
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
````

> Примечание по якорям: GitHub генерирует якоря из заголовков, убирая скобки и пробелы. Например `### [superpowers](https://github.com/obra/superpowers)` превращается в `#superpowersgithubcomobrasuperpowers`. Ссылки в блоке "Что тебе нужно?" используют эти якоря.

- [ ] **Step 2: Verify file exists**

Run:
```bash
ls -la /c/Users/Bokti/Desktop/claude-arsenal/README.md
```
Expected: file exists, non-zero size.

- [ ] **Step 3: Commit**

```bash
cd /c/Users/Bokti/Desktop/claude-arsenal
git add README.md
git commit -m "feat: add root README with 'what do you need?' navigation"
```

Expected: commit succeeds, `git log` shows 4 commits total.

---

## Task 4: Add CONTRIBUTING.md and issue template

**Files:**
- Create: `CONTRIBUTING.md`
- Create: `.github/ISSUE_TEMPLATE/add-resource.yml`
- Create: `.github/ISSUE_TEMPLATE/config.yml` (optional — direct "Open blank issue" off)

- [ ] **Step 1: Write `CONTRIBUTING.md`**

Create `C:\Users\Bokti\Desktop\claude-arsenal\CONTRIBUTING.md`:

````markdown
# Как добавить ресурс в claude-arsenal

Спасибо, что хочешь добавить крутой ресурс! Это займёт меньше минуты.

## Вариант A — через Issue (быстрее, не требует git)

1. Нажми [Create new issue → Добавить ресурс](../../issues/new/choose).
2. Заполни форму (ссылка, категория, "что даёт", "когда брать", "для чего лучше").
3. Отправь — maintainer перенесёт в README соответствующей папки.

## Вариант B — через Pull Request

### 1. Найди нужную папку

| Что это | Куда |
|---|---|
| Целая методология (всё-в-одном, skills+hooks+commands) | `frameworks/` |
| Многоагентная система, оркестратор | `orchestrators/` |
| Один агент или один скилл | `agents-skills/` |
| MCP сервер, CLI инструмент, утилита | `tools/` |
| Хук, шаблон CLAUDE.md, промпт | `automation/` |
| Гайд, шпаргалка, заметка | `docs/` |

### 2. Открой README этой папки и добавь карточку в конец секции "Ресурсы"

Шаблон (копируй и заполняй):

```markdown
### [название](https://github.com/user/repo)

**Что даёт:** одно предложение про полезность
**Когда брать:** одно предложение про use-case
**Для чего лучше:** универсал / backend / frontend / mobile / data
**Установка:** команда клона или ссылка на инструкцию
**Автор:** [@username](https://github.com/username)
```

**Поля:**
- **Что даёт** — максимум одно предложение, ориентированное на пользу.
- **Когда брать** — одно предложение про конкретную ситуацию.
- **Для чего лучше** — одно или несколько из: `универсал`, `backend`, `frontend`, `mobile`, `data`.
- **Установка** — рабочая команда (обычно `git clone ...`) или ссылка на инструкцию в репо.
- **Автор** — ссылка на GitHub профиль автора ресурса.

### 3. Сделай Pull Request

- Название PR: `feat: add <название ресурса> to <папка>`
- В описании PR: одна строка зачем.

## Правила

- ✅ **Только публичные репо** с открытой лицензией (MIT, Apache, GPL, BSD и т.п.).
- ✅ **Атрибуция автора обязательна** (поле "Автор" с ссылкой).
- ✅ **Ресурс должен работать** — не добавляй заброшенные проекты без коммитов за последний год, если только это не "классика".
- ❌ **Не дублируй** — проверь, что такого ещё нет в репо.
- ❌ **Не копируй код** из оригинального репо сюда — только ссылки и описания.

## Вопросы?

Заведи [discussion](../../discussions) или issue.
````

- [ ] **Step 2: Write issue template `add-resource.yml`**

Create directory and file:

```bash
mkdir -p /c/Users/Bokti/Desktop/claude-arsenal/.github/ISSUE_TEMPLATE
```

Create `C:\Users\Bokti\Desktop\claude-arsenal\.github\ISSUE_TEMPLATE\add-resource.yml`:

```yaml
name: Добавить ресурс
description: Предложи репо, инструмент, агента или гайд в claude-arsenal
title: "[Resource] <название>"
labels: ["new-resource"]
body:
  - type: markdown
    attributes:
      value: |
        Спасибо! Заполни форму — maintainer перенесёт карточку в нужную папку.

  - type: input
    id: repo-url
    attributes:
      label: Ссылка на репо или ресурс
      placeholder: https://github.com/user/repo
    validations:
      required: true

  - type: dropdown
    id: category
    attributes:
      label: Категория
      description: К какой папке относится ресурс?
      options:
        - frameworks (методология всё-в-одном)
        - orchestrators (многоагентная система)
        - agents-skills (один агент или скилл)
        - tools (MCP сервер, утилита)
        - automation (хук, шаблон, промпт)
        - docs (гайд, шпаргалка)
    validations:
      required: true

  - type: textarea
    id: what-gives
    attributes:
      label: Что даёт
      description: Одно предложение про полезность.
      placeholder: "Полный workflow разработки — брейншторм, планирование, TDD, код-ревью"
    validations:
      required: true

  - type: textarea
    id: when-use
    attributes:
      label: Когда брать
      description: Одно предложение про use-case.
      placeholder: "Если хочешь отстроенный процесс, а не собирать всё с нуля"
    validations:
      required: true

  - type: dropdown
    id: domain
    attributes:
      label: Для чего лучше
      multiple: true
      options:
        - универсал
        - backend
        - frontend
        - mobile
        - data
    validations:
      required: true

  - type: input
    id: install
    attributes:
      label: Установка
      description: Команда клона или ссылка на инструкцию.
      placeholder: "git clone https://github.com/user/repo ~/.claude/plugins/"

  - type: input
    id: author
    attributes:
      label: Автор (GitHub username)
      placeholder: "@username"
    validations:
      required: true
```

- [ ] **Step 3: Write issue template config `config.yml`**

Create `C:\Users\Bokti\Desktop\claude-arsenal\.github\ISSUE_TEMPLATE\config.yml`:

```yaml
blank_issues_enabled: true
contact_links:
  - name: Вопрос или обсуждение
    url: https://github.com/Baktiyar88/claude-arsenal/discussions
    about: Для общих вопросов используй Discussions, а не Issues.
```

- [ ] **Step 4: Verify files**

Run:
```bash
ls -la /c/Users/Bokti/Desktop/claude-arsenal/CONTRIBUTING.md \
       /c/Users/Bokti/Desktop/claude-arsenal/.github/ISSUE_TEMPLATE/add-resource.yml \
       /c/Users/Bokti/Desktop/claude-arsenal/.github/ISSUE_TEMPLATE/config.yml
```
Expected: all 3 files listed.

- [ ] **Step 5: Commit**

```bash
cd /c/Users/Bokti/Desktop/claude-arsenal
git add CONTRIBUTING.md .github/
git commit -m "feat: add CONTRIBUTING guide and issue template for new resources"
```

Expected: commit succeeds, `git log` shows 5 commits total.

---

## Task 5: Final verification and push

**Files:** none created; only verification and push.

- [ ] **Step 1: Verify full file tree**

Run:
```bash
cd /c/Users/Bokti/Desktop/claude-arsenal
find . -type f -not -path './.git/*' | sort
```

Expected output (exact list):
```
./.github/ISSUE_TEMPLATE/add-resource.yml
./.github/ISSUE_TEMPLATE/config.yml
./.gitignore
./CONTRIBUTING.md
./LICENSE
./README.md
./agents-skills/README.md
./automation/README.md
./docs/README.md
./docs/superpowers/plans/2026-04-21-claude-arsenal-scaffold.md
./docs/superpowers/specs/2026-04-21-claude-arsenal-structure-design.md
./frameworks/README.md
./orchestrators/README.md
./tools/README.md
```

14 files total. If any missing, go back to the corresponding task and fix.

- [ ] **Step 2: Verify git log**

Run:
```bash
cd /c/Users/Bokti/Desktop/claude-arsenal
git log --oneline
```

Expected: 5 commits in order (newest first):
```
<hash> feat: add CONTRIBUTING guide and issue template for new resources
<hash> feat: add root README with 'what do you need?' navigation
<hash> feat: add 6 category READMEs with initial resources (superpowers, graphify)
<hash> chore: add MIT LICENSE and .gitignore
<hash> docs: add design spec for claude-arsenal structure
```

- [ ] **Step 3: Verify working tree is clean**

Run:
```bash
cd /c/Users/Bokti/Desktop/claude-arsenal
git status
```

Expected: `nothing to commit, working tree clean`.

- [ ] **Step 4: Commit this plan file itself**

Since the plan is inside the repo tree, it should also be committed:

```bash
cd /c/Users/Bokti/Desktop/claude-arsenal
git add docs/superpowers/plans/2026-04-21-claude-arsenal-scaffold.md
git commit -m "docs: add implementation plan for initial scaffold"
```

(If the plan was already committed earlier in the session, `git status` will show clean and this step is a no-op. Skip it in that case.)

- [ ] **Step 5: Ask user before pushing**

**IMPORTANT:** Pushing to `origin/main` on a public repo is a shared-state action. Before pushing, confirm with the user:

> "Готов запушить 6 коммитов на `origin/main` (https://github.com/Baktiyar88/claude-arsenal). Пушим?"

Wait for explicit user approval. Do **NOT** push without confirmation.

- [ ] **Step 6: Push to origin/main**

After user confirms:

```bash
cd /c/Users/Bokti/Desktop/claude-arsenal
git push -u origin main
```

Expected: push succeeds, upstream set to `origin/main`.

- [ ] **Step 7: Verify on GitHub**

Open https://github.com/Baktiyar88/claude-arsenal in browser. Verify:
- [x] README.md renders with "🎯 Что тебе нужно?" section
- [x] All 6 folders visible with their READMEs
- [x] CONTRIBUTING.md linked from root README works
- [x] Issues → "New issue" shows "Добавить ресурс" template
- [x] Internal links (`frameworks/README.md#superpowers...`) click through correctly

If anything looks broken, capture what's wrong and open a fix-up commit in a follow-up task.

---

## Self-Review (done before handing off)

**Spec coverage check:**
- ✅ G1 (10-sec navigation) — Task 3 root README with "что тебе нужно?" block
- ✅ G2 (< 1 min to add) — Task 4 issue template with form fields
- ✅ G3 (unified card format) — Template present in all 6 folder READMEs + CONTRIBUTING
- ✅ G4 (scales 5 to 100+) — No per-resource coupling; folders are append-only
- ✅ G5 (licenses + attribution) — MIT in LICENSE, rules in CONTRIBUTING, Автор field in card
- ✅ 6 folders — Task 2 creates all 6
- ✅ Root README — Task 3
- ✅ CONTRIBUTING — Task 4
- ✅ Issue template — Task 4
- ✅ LICENSE + .gitignore — Task 1
- ✅ Commit + push — Task 5

**Placeholder scan:** no TBDs, every file has full content inline.

**Type/name consistency:** folder names consistent (`frameworks`, `orchestrators`, `agents-skills`, `tools`, `automation`, `docs`) across: spec, all tasks, root README table, CONTRIBUTING table, issue template dropdown. Card field names consistent (`Что даёт`, `Когда брать`, `Для чего лучше`, `Установка`, `Автор`) across all 6 folder READMEs and CONTRIBUTING.

**Known limitation:** GitHub anchor generation for headings containing links is non-deterministic across renderers. If links in the root README don't jump correctly after push (Step 7), fix in a follow-up by either (a) adjusting anchors after inspecting GitHub's rendering, or (b) switching to `<a id="...">` explicit anchors above each card.
