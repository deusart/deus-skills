# AGENTS.md

## Как запускать

- проверка: `node tools/check-docs.mjs`

## Правила

- скилл: `skills/<name>/SKILL.md`, `name` = имя папки, `description` = триггеры
- имена: `docs/rules/naming-convention.md`
- документы: паспорт и индекс, `docs/index.md`
- заглушки и разделы «позже» запрещены

## Как проверять

`node tools/check-docs.mjs` возвращает 0 или список ошибок с путями.
