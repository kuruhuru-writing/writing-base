# Спецификация пакета контекста для ИИ-агента

## Назначение

Пакет контекста — это набор файлов, который позволяет агенту понять текущее состояние романа и дать полезный ответ.

## Минимальный пакет

Для вопроса “что дальше?”:

```text
00-method/hybrid-novel-method.md
01-planning/compass.md
01-planning/beacons.md
01-planning/promises.md
01-planning/questions.md
01-planning/decisions.md
03-journal/writing-log.md
02-manuscript/scenes/<последние 3–5 сцен>
```

## Для проверки сцены

```text
00-method/hybrid-novel-method.md
checklists/scene-checklist.md
01-planning/compass.md
01-planning/beacons.md
01-planning/promises.md
01-planning/questions.md
02-manuscript/scenes/<проверяемая сцена>
02-manuscript/scenes/<предыдущая сцена, если есть>
```

## Для планирования главы

```text
00-method/hybrid-novel-method.md
01-planning/compass.md
01-planning/beacons.md
01-planning/promises.md
01-planning/questions.md
01-planning/decisions.md
03-journal/writing-log.md
02-manuscript/scenes/<последние сцены>
```

## Для аудита непрерывности

```text
01-planning/*
02-manuscript/scenes/*
03-journal/*
```

Если рукопись большая, можно дать собранный `04-output/manuscript.md` и planning-файлы.

## Как агент должен отвечать

Агент должен указывать:

- на какие файлы он опирается;
- что считает фактом;
- где делает предположение;
- какие файлы надо обновить;
- какие варианты доступны автору.
