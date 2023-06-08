---
title: FormatConditionCollection.AddCondition
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection method. Adds a formatting condition
type: docs
url: /net/aspose.cells/formatconditioncollection/addcondition/
---
## AddCondition(FormatConditionType, OperatorType, string, string) {#addcondition_1}

Adds a formatting condition.

```csharp
public int AddCondition(FormatConditionType type, OperatorType operatorType, string formula1, 
    string formula2)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | FormatConditionType | The type of format condition. |
| operatorType | OperatorType | The operator type |
| formula1 | String | The value or expression associated with conditional formatting. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | String | The value or expression associated with conditional formatting. The input format is same with formula1 |

### Return Value

Formatting condition object index;

### See Also

* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCondition(FormatConditionType) {#addcondition}

Add a format condition.

```csharp
public int AddCondition(FormatConditionType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | FormatConditionType | Format condition type. |

### Return Value

Formatting condition object index;

### See Also

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


