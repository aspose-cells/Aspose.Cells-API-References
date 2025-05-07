---
title: Validation.InputTitle
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the title of the datavalidation input dialog box
type: docs
url: /net/aspose.cells/validation/inputtitle/
---
## Validation.InputTitle property

Represents the title of the data-validation input dialog box.

```csharp
public string InputTitle { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(null, validation.InputTitle, foldName, className, caseName);
private void Property_InputTitle(Validation validation)
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


