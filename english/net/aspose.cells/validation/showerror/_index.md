---
title: Validation.ShowError
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Indicates whether the data validation error message will be displayed whenever the user enters invalid data
type: docs
url: /net/aspose.cells/validation/showerror/
---
## Validation.ShowError property

Indicates whether the data validation error message will be displayed whenever the user enters invalid data.

```csharp
public bool ShowError { get; set; }
```

### Examples

```csharp
// Called: target.ShowError = source.ShowError;
private static void Validation_Property_ShowError(Validation source, Validation target)
        {
            target.AlertStyle = source.AlertStyle;
            target.ErrorMessage = source.ErrorMessage;
            target.ErrorTitle = source.ErrorTitle;
            target.Formula1 = source.Formula1;
            target.Formula2 = source.Formula2;
            target.IgnoreBlank = source.IgnoreBlank;
            target.InCellDropDown = source.InCellDropDown;
            target.InputMessage = source.InputMessage;
            target.InputTitle = source.InputTitle;
            target.Operator = source.Operator;
            target.ShowError = source.ShowError;
            target.ShowInput = source.ShowInput;
            target.Type = source.Type;
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


