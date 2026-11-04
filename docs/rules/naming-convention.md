---
id: RULE-001
title: "Соглашение об именах"
type: rule
status: actual
owner: architect
date: 2026-11-04
---

# Соглашение об именах

## Файлы и папки

- английский, без транслита, kebab-case
- имя описывает содержимое: `check-docs.mjs`, не `check.mjs`
- без пробелов и длинных тире
- скилл: `skills/<name>/SKILL.md`, `<name>` совпадает с полем `name`

## Документы

| Тип | Формат | Папка |
|-----|--------|-------|
| spec | `SPEC-001` | `docs/specs` |
| adr | `ADR-0001` | `docs/adr` |
| rule | `RULE-001` | `docs/rules` |
| review | `REV-001` | `docs/reviews` |
| concept | `CONCEPT` | `docs/concept` |
| glossary | `GLOSSARY` | `docs/glossary.md` |

Имя файла: `<ID>-<slug>.md`.

## Ветки

`main` основная. Рабочие: `feat/<slug>`, `fix/<slug>`, `docs/<slug>`, `chore/<slug>`.

## Коммиты

Conventional Commits: `<type>(<scope>): <subject>`, subject английский, императив, до
72 символов.

## Язык

Текст документов и скиллов русский. Имена файлов, коммиты и код английские.
