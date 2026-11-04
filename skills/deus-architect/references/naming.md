# Naming

Домен имена. Артефакт в проекте: `docs/rules/naming-convention.md`.

## Файлы и папки

- английский, без транслита, kebab-case
- имя описывает содержимое: `user-profile.md`, не `up.md`
- без пробелов, без длинных тире, без дат в имени
- расширение `.md` у документов, `.mjs` или `.py` у скриптов
- папки: `docs/rules`, `docs/specs`, `docs/tasks`, `tools`, `skills`, `agents`

## Документы и идентификаторы

| Тип | Формат | Папка |
|-----|--------|-------|
| spec | `SPEC-001` | `docs/specs` |
| adr | `ADR-0001` | `docs/adr` |
| rule | `RULE-001` | `docs/rules` |
| review | `REV-001` | `docs/reviews` |
| task | `TASK-001` | `docs/tasks` |
| concept | `CONCEPT`, `MVP` | `docs/concept` |
| glossary | `GLOSSARY` | `docs/glossary.md` |

Имя файла: `<ID>-<slug>.md`, например `SPEC-001-solution-architecture.md`.
Ширина номера фиксирована внутри типа: три цифры у spec и rule, четыре у adr.
Пропусков в нумерации нет.

## Ветки

`main` основная. Рабочие: `feat/<slug>`, `fix/<slug>`, `docs/<slug>`, `chore/<slug>`.
Долгих веток нет, тема живёт до merge.

## Коммиты

Conventional Commits: `<type>(<scope>): <subject>`.

- типы: `feat`, `fix`, `docs`, `chore`, `refactor`, `test`, `ci`
- subject английский, императив, до 72 символов, без точки на конце
- тело только если нужно объяснить почему

## PR и MR

Заголовок в формате коммита. Тело: что меняется, зачем, как проверено, что не входит.

## Язык

Текст документов русский. Идентификаторы, имена файлов, код, коммиты английские.
Смешение внутри одного имени не допускается.

## Проверка

`tools/check-docs.mjs` валидирует имена файлов: латиница, kebab-case, без длинных тире.
Имена с кириллицей или пробелом это ошибка, а не предупреждение.
