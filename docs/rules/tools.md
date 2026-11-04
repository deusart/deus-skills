---
id: RULE-002
title: "Расширения Obsidian"
type: rule
status: actual
owner: architect
date: 2026-11-04
---

# Расширения Obsidian

Vault это корень проекта, заметки лежат в `docs/`. Конфигурация в `.obsidian/` рядом с
`README.md`. Так имя vault совпадает с именем проекта, а пути `docs/rules`, `docs/specs`
и `docs/index.md` остаются прежними.

## Тема

Minimal. Выбор зафиксирован в `.obsidian/appearance.json`: `"theme": "obsidian"`,
`"cssTheme": "Minimal"`. Тема лежит в репозитории целиком, `.obsidian/themes/Minimal`.

## Расширения

| Плагин | Идентификатор | Зачем |
|--------|---------------|-------|
| Kanban | `obsidian-kanban` | доска `docs/tasks/board.md` |
| Dataview | `dataview` | запросы по паспортам документов |
| Minimal Theme Settings | `obsidian-minimal-settings` | настройки темы Minimal |

Список зафиксирован в `.obsidian/community-plugins.json`.

## Фильтры

Obsidian не индексирует код и служебные файлы. Список в `.obsidian/app.json` →
`userIgnoreFilters`: `archive/`, `skills/`, `tools/`, `src/`, `AGENTS.md`, `README.md`,
`.gitignore`, `.gitattributes`, `.deus-architect.yaml`. Новые заметки по умолчанию
создаются в `docs/` (`newFileFolderPath`).

## Установка

Settings → Community plugins → Browse → найти по идентификатору, установить, включить.
Тема уже в репозитории, ставить её не нужно. Код плагинов не коммитится: после
клонирования они ставятся один раз вручную. Без них страницы открываются как обычный
markdown, данные не теряются.
