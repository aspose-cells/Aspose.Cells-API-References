---
title: Add
second_title: Справочник по Aspose.Cells для .NET API
description: Добавляет условие форматирования и диапазон ячеек в FormatConditions FormatConditions может содержать до трех условных форматов. В формулах условного форматирования не допускаются ссылки на другие листы.
type: docs
weight: 40
url: /ru/net/aspose.cells/formatconditioncollection/add/
---
## FormatConditionCollection.Add method

Добавляет условие форматирования и диапазон ячеек в FormatConditions FormatConditions может содержать до трех условных форматов. В формулах условного форматирования не допускаются ссылки на другие листы.

```csharp
public int[] Add(CellArea cellArea, FormatConditionType type, OperatorType operatorType, 
    string formula1, string formula2)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellArea | CellArea | Диапазон ячеек с условным форматированием. |
| type | FormatConditionType | Тип условного форматирования. Может быть одним из членов FormatConditionType. |
| operatorType | OperatorType | Оператор сравнения. Он может быть одним из членов OperatorType. |
| formula1 | String | Значение или выражение, связанное с условным форматированием. |
| formula2 | String | Значение или выражение, связанное с условным форматированием |

### Возвращаемое значение

[0]: индекс объекта условия форматирования; [1] индекс ранга ячейки.

### Смотрите также

* struct [CellArea](../../cellarea)
* enum [FormatConditionType](../../formatconditiontype)
* enum [OperatorType](../../operatortype)
* class [FormatConditionCollection](../../formatconditioncollection)
* пространство имен [Aspose.Cells](../../formatconditioncollection)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
