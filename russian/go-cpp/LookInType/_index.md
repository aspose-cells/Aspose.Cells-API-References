---
title: "Перечисление LookInType"
linktitle: "LookInType"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Перечисление LookInType. Инкапсулирует объект, представляющий lookintype в Go."
type: docs
weight: 200
url: /ru/go-cpp/lookintype/
---

## LookInType Enum

Представляет тип «look in».

```go

type LookInType int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [Formulas](./formulas/) | Находит искомый объект из формулы(<see cref=\"Cell.Formula\"/>), если ячейка содержит формулу, иначе ищет из исходного значения ячейки (то же, что и <see cref=\"OriginalValues\"/>). |
| [Values](./values/) | Находит объект из исходного значения ячейки(<see cref=\"Cell.Value\"/>) и отформатированного значения(<see cref=\"Cell.StringValue\"/>). |
| [ValuesExcludeFormulaCell](./valuesexcludeformulacell/) | Игнорирует ячейки, содержащие формулу. Для ячеек, не содержащих формулу, это то же самое, что <see cref=\"Values\"/>. |
| [Comments](./comments/) | Находит объект только из комментария ячейки. Игнорирует ячейки без комментария. |
| [OnlyFormulas](./onlyformulas/) | Игнорирует ячейки, не содержащие формулу. Для ячеек, содержащих формулу, ищет искомый объект из формулы(<see cref=\"Cell.Formula\"/>). |
| [OriginalValues](./originalvalues/) | Находит объект только из исходного значения ячейки. |
| [FormattedValues](./formattedvalues/) | Находит объект только из отформатированного значения(<see cref=\"Cell.StringValue\"/>) ячейки. |
