---
title: FormatConditionCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection method. Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting
type: docs
url: /net/aspose.cells/formatconditioncollection/add/
---
## FormatConditionCollection.Add method

Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting.

```csharp
public int[] Add(CellArea cellArea, FormatConditionType type, OperatorType operatorType, 
    string formula1, string formula2)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Conditional formatted cell range. |
| type | FormatConditionType | Type of conditional formatting.It could be one of the members of FormatConditionType. |
| operatorType | OperatorType | Comparison operator.It could be one of the members of OperatorType. |
| formula1 | String | The value or expression associated with conditional formatting. |
| formula2 | String | The value or expression associated with conditional formatting |

### Return Value

[0]:Formatting condition object index;[1] Effected cell rang index.

### See Also

* struct [CellArea](../../cellarea/)
* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


