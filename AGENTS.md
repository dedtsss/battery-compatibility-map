# Battery Compatibility Map — agent rules

## Обязательный язык публикаций GitHub

**Весь новый авторский человекочитаемый текст, публикуемый в GitHub от имени владельца, писать по-русски.** Это относится к названиям и описаниям задач, запросам на слияние, комментариям и отзывам, этапам и результатам исполнения, сообщениям коммитов, отчётам, журналам, документации и авторским пояснениям в коде. Перед публикацией проверять язык и исправлять английские шаблонные фразы. Не переводить программные идентификаторы, имена и пути, команды, параметры, API, машинные статусы (`RUN_STARTED`, `SUCCESS`, `BLOCKED` и др.), код и дословные внешние цитаты, если перевод нарушает точность или совместимость. Исключения — только по явному указанию владельца либо при строгой технической необходимости. Исторические записи массово не переписывать. Общее обязательное правило: [политика русского языка](https://github.com/dedtsss/agent-dispatch/blob/main/docs/memory/github-russian-language-policy.md).

This is the canonical rule file. Read the task/Issue, this file, and only relevant files.

- Make the smallest correct change on a focused branch; preserve unrelated work and avoid speculative features or broad refactors.
- Treat `data/relations.csv` as user-reported practical evidence, not manufacturer fact. Do not invent compatibility, adapter behaviour, electrical safety, or protection details.
- Keep uncertainty and warnings about connector shape, polarity, contacts, thermistor/ID pins, current capability, over-discharge, and overheating protection unless evidence justifies changing them.
- Prefer surgical data changes and keep the site static unless the task explicitly requires otherwise.
- Do not expose or commit secrets or private data; do not merge or change deployment without explicit authorization.

Inspect changed pages/tables in a browser when practical. If no automated test applies, say so and report exact manual validation and remaining risks.
