---
title: Workbook.UpdateCustomFunctionDefinition
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Updates definition of custom functions
type: docs
url: /net/aspose.cells/workbook/updatecustomfunctiondefinition/
---
## Workbook.UpdateCustomFunctionDefinition method

Updates definition of custom functions.

```csharp
public void UpdateCustomFunctionDefinition(CustomFunctionDefinition definition)
```

| Parameter | Type | Description |
| --- | --- | --- |
| definition | CustomFunctionDefinition | Special definition of custom functions for user's special requirement. |

### Remarks

This method can be used for some special scenarios. For example, if user needs some parameters of some custom functions be calculated in array mode, then user may provide their own definition with implemented [`GetArrayModeParameters`](../../customfunctiondefinition/getarraymodeparameters/) for those functions. After the data of formulas being updated, those specified parameters will be calculated in array mode automatically when calculating corresponding custom functions.

### See Also

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


