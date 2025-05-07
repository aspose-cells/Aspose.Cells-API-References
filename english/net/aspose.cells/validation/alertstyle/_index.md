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
// Called: target.AlertStyle = source.AlertStyle;
private static void Property_AlertStyle(Validation source, Validation target)
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

* enum [ValidationAlertType](../../validationalerttype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


