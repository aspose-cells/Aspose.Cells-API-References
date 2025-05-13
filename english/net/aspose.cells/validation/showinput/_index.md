---
title: Validation.ShowInput
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range
type: docs
url: /net/aspose.cells/validation/showinput/
---
## Validation.ShowInput property

Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range.

```csharp
public bool ShowInput { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(true, validation.ShowInput, foldName, className, caseName);
private void Validation_Property_ShowInput(Validation validation)
        {
            AssertHelper.AreEqual("Yes,No", validation.Formula1, foldName, className, caseName);
            AssertHelper.AreEqual(ValidationType.List, validation.Type, foldName, className, caseName);
            AssertHelper.AreEqual(true, validation.IgnoreBlank, foldName, className, caseName);
            AssertHelper.AreEqual(true, validation.InCellDropDown, foldName, className, caseName);
            AssertHelper.AreEqual(true, validation.ShowInput, foldName, className, caseName);
            AssertHelper.AreEqual(null, validation.InputTitle, foldName, className, caseName);
            AssertHelper.AreEqual(null, validation.InputMessage, foldName, className, caseName);
            AssertHelper.AreEqual(true, validation.ShowError, foldName, className, caseName);
            AssertHelper.AreEqual(ValidationAlertType.Stop, validation.AlertStyle, foldName, className, caseName);
            AssertHelper.AreEqual(null, validation.ErrorTitle, foldName, className, caseName);
            AssertHelper.AreEqual(null, validation.ErrorMessage, foldName, className, caseName);
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


