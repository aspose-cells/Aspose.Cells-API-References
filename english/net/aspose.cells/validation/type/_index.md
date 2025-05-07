---
title: Validation.Type
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the data validation type
type: docs
url: /net/aspose.cells/validation/type/
---
## Validation.Type property

Represents the data validation type.

```csharp
public ValidationType Type { get; set; }
```

### Examples

```csharp
// Called: if(valSrc.Type != ValidationType.List)
public static void Property_Type(Validation valSrc, Validation valDest, string info)
        {
            if (AssertHelper.checkNull(valSrc, valDest, info))
            {
                return;
            }
            //Settings
            AssertHelper.AreEqual(valSrc.Type, valDest.Type, info + ".Type");
            if(valSrc.Type != ValidationType.List)
                AssertHelper.AreEqual(valSrc.Operator, valDest.Operator, info + ".Operator");
            AssertHelper.AreEqual(valSrc.IgnoreBlank, valDest.IgnoreBlank, info + ".IgnoreBlank");
            AssertHelper.AreEqual(valSrc.InCellDropDown, valDest.InCellDropDown, info + ".InCellDropDown");
            AssertHelper.AreEqual(valSrc.Formula1, valDest.Formula1, info + ".Formula1");
            AssertHelper.AreEqual(valSrc.Formula2, valDest.Formula2, info + ".Formula2");
            //Input message
            AssertHelper.AreEqual(valSrc.InputTitle, valDest.InputTitle, info + ".InputTitle");
            AssertHelper.AreEqual(valSrc.InputMessage, valDest.InputMessage, info + ".InputMessage");
            //Error alert
            AssertHelper.AreEqual(valSrc.AlertStyle, valDest.AlertStyle, info + ".AlertStyle");
            AssertHelper.AreEqual(valSrc.ErrorTitle, valDest.ErrorTitle, info + ".ErrorTitle");
            AssertHelper.AreEqual(valSrc.ErrorMessage, valDest.ErrorMessage, info + ".ErrorMessage");
        }
```

### See Also

* enum [ValidationType](../../validationtype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


