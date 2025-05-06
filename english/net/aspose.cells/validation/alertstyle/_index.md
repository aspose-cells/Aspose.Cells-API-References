---
title: Validation.AlertStyle
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the validation alert style
type: docs
url: /net/aspose.cells/validation/alertstyle/
---
## Validation.AlertStyle property

Represents the validation alert style.

```csharp
public ValidationAlertType AlertStyle { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(ValidationAlertType.Stop, validation.AlertStyle, &amp;quot;validation.AlertStyle&amp;quot;);
private void Property_AlertStyle(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            AssertHelper.AreEqual(1, sheet.Validations.Count, &quot;sheet.Validations.Count&quot;);
            Validation validation = sheet.Validations[0];
            AssertHelper.AreEqual(ValidationAlertType.Stop, validation.AlertStyle, &quot;validation.AlertStyle&quot;);
        }
```

### See Also

* enum [ValidationAlertType](../../validationalerttype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


