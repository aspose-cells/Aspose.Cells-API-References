---
title: Validation.InputMessage
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the data validation input message
type: docs
url: /net/aspose.cells/validation/inputmessage/
---
## Validation.InputMessage property

Represents the data validation input message.

```csharp
public string InputMessage { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual("", validation.InputMessage, foldName, className, caseName);
private void Validation_Property_InputMessage(Validation validation)
        {
            AssertHelper.AreEqual("Yes,No", validation.Formula1, foldName, className, caseName);
            AssertHelper.AreEqual(ValidationType.List, validation.Type, foldName, className, caseName);
            AssertHelper.AreEqual(true, validation.IgnoreBlank, foldName, className, caseName);
            AssertHelper.AreEqual(true, validation.InCellDropDown, foldName, className, caseName);
            AssertHelper.AreEqual(true, validation.ShowInput, foldName, className, caseName);
            AssertHelper.AreEqual("", validation.InputTitle, foldName, className, caseName);
            AssertHelper.AreEqual("", validation.InputMessage, foldName, className, caseName);
            AssertHelper.AreEqual(true, validation.ShowError, foldName, className, caseName);
            AssertHelper.AreEqual(ValidationAlertType.Stop, validation.AlertStyle, foldName, className, caseName);
            AssertHelper.AreEqual("", validation.ErrorTitle, foldName, className, caseName);
            AssertHelper.AreEqual("", validation.ErrorMessage, foldName, className, caseName);
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


