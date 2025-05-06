---
title: Worksheet.Validations
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the data validation setting collection in the worksheet
type: docs
url: /net/aspose.cells/worksheet/validations/
---
## Worksheet.Validations property

Gets the data validation setting collection in the worksheet.

```csharp
public ValidationCollection Validations { get; }
```

### Examples

```csharp
// Called: Validation validation = sheet.Validations[0];
private void Property_Validations(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[1];
            AssertHelper.AreEqual(1, sheet.Validations.Count, &quot;sheet.Validations.Count&quot;);
            Validation validation = sheet.Validations[0];
            AssertHelper.AreEqual(ValidationAlertType.Stop, validation.AlertStyle, &quot;validation.AlertStyle&quot;);
        }
```

### See Also

* class [ValidationCollection](../../validationcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


