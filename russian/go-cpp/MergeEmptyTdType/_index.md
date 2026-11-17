---
title: "Перечисление MergeEmptyTdType"
linktitle: "MergeEmptyTdType"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Перечисление MergeEmptyTdType. Инкапсулирует объект, представляющий mergeemptytdtype в Go."
type: docs
weight: 200
url: /ru/go-cpp/mergeemptytdtype/
---

## MergeEmptyTdType Enum

Представляет тип объединения для пустого элемента TD при экспорте файла в HTML.

```go

type MergeEmptyTdType int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [Default](./default/) | Отображать как MS Excel. |
| [None](./none/) | Пустые элементы TD не будут объединяться при экспорте файла в html. Это приведёт к значительно большему html‑файлу. |
| [MergeForcely](./mergeforcely/) | Принудительное объединение пустых элементов TD при экспорте файла в html. Размер html‑файла будет значительно уменьшен после установки значения в true. Если вы хотите импортировать html‑файл в Excel или экспортировать идеальные линии сетки при сохранении файла в html, оставьте значение по умолчанию. |
