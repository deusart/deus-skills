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
| Kanban | `kanban` | доска `docs/tasks/board.md` |
| Dataview | `dataview` | запросы по паспортам документов |
| Minimal Theme Settings | `obsidian-minimal-settings` | настройки темы Minimal |

Список зафиксирован в `docs/.obsidian/community-plugins.json`.

## Установка

Settings → Community plugins → Browse → найти по идентификатору, установить, включить.
Код плагинов и тема в репозиторий не коммитятся: после клонирования они ставятся один
раз вручную. Без них страницы открываются как обычный markdown, данные не теряются.
