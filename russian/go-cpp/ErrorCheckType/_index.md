---
title: "Перечисление ErrorCheckType"
linktitle: "ErrorCheckType"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Перечисление ErrorCheckType. Инкапсулирует объект, представляющий errorchecktype в Go."
type: docs
weight: 200
url: /ru/go-cpp/errorchecktype/
---

## ErrorCheckType Enum

Представляет все типы проверки ошибок.

```go

type ErrorCheckType int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [EvaluationError](./evaluationerror/) | Игнорировать ошибки, когда ячейки содержат формулы, приводящие к ошибке. |
| [EmptyCellRef](./emptycellref/) | Игнорировать ошибки, когда формулы ссылаются на пустые ячейки. |
| [NumberStoredAsText](./numberstoredastext/) | Игнорировать ошибки, когда числа отформатированы как текст или предваряются апострофом |
| [InconsistRange](./inconsistrange/) | Игнорировать ошибки, когда формулы пропускают определённые ячейки в области. |
| [InconsistFormula](./inconsistformula/) | Игнорировать ошибки, когда формула в области вашего листа отличается от других формул в той же области. |
| [TwoDigitTextYear](./twodigittextyear/) | Игнорировать ошибки, когда формулы содержат ячейки, отформатированные как текст, с годами, представленными двумя цифрами. |
| [UnlockedFormula](./unlockedformula/) | Игнорировать ошибки, когда разблокированные ячейки содержат формулы. |
| [TableDataValidation](./tabledatavalidation/) | Игнорировать ошибки, когда значение ячейки в таблице не соответствует указанным правилам проверки данных. |
| [CalculatedColumn](./calculatedcolumn/) | Игнорировать ошибки, когда ячейки содержат значение, отличающееся от вычисленной формулы столбца. |
