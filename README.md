# deus-skills

Репозиторий скиллов Deus. Агентская среда, правила и проверка живут здесь же.

## Что внутри

| Путь | Назначение |
|------|------------|
| [skills/deus-architect](skills/deus-architect/SKILL.md) | архитектор солюшна |
| [skills/deus-de](skills/deus-de/SKILL.md) | инженер данных: пайплайны, хранилище, dbt, Airflow |
| [skills/deus-devops](skills/deus-devops/SKILL.md) | инфраструктура: окружения, CI/CD, секреты, бэкапы |
| [archive/deus-architect-v1](archive/deus-architect-v1/SKILL.md) | первая версия, сохранена как история |
| [docs/rules](docs/rules/naming-convention.md) | правила репозитория |
| [tools](tools/check-docs.mjs) | проверка документации и скиллов |

## Как добавить скилл

1. `skills/<name>/SKILL.md`: `name` равен имени папки, `description` описывает только
   триггеры, без пересказа процесса.
2. Тяжёлое в `references/`, исполняемое в `scripts/`.
3. Записать скилл в `docs/index.md`.
4. `node tools/check-docs.mjs`.

## Проверка

```
node tools/check-docs.mjs
```

Проверяет паспорта документов, уникальность `id`, `title` = H1, обязательные разделы,
покрытие индекса, живые ссылки, заглушки, имена файлов и frontmatter скиллов.
Первый прогон на незнакомом репозитории идёт в режиме знакомства, `--strict` включает
строгий режим.
