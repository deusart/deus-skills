---
id: RULE-002
title: "Расширения Obsidian"
type: rule
status: actual
owner: architect
date: 2026-11-04
---

# Расширения Obsidian

Vault `docs/` рассчитан на три расширения и тему Minimal.

## Тема

Minimal. Ставится через Settings → Appearance → Themes → Manage → Minimal. Выбор темы
зафиксирован в `docs/.obsidian/appearance.json`.

## Расширения

| Плагин | Идентификатор | Зачем |
|--------|---------------|-------|
| Kanban | `obsidian-kanban` | доска `docs/tasks/board.md` |
| Dataview | `dataview` | запросы по паспортам документов |
| Minimal Theme Settings | `obsidian-minimal-settings` | настройки темы Minimal |

Список зафиксирован в `docs/.obsidian/community-plugins.json`. Тема Minimal лежит в
репозитории целиком: `docs/.obsidian/themes/Minimal`.

## Установка

Settings → Community plugins → Browse → найти по идентификатору, установить, включить.
Тема Minimal уже в репозитории, ставить её не нужно. Код плагинов не коммитится: после
клонирования они ставятся один раз вручную. Без них страницы открываются как обычный
markdown, данные не теряются.
