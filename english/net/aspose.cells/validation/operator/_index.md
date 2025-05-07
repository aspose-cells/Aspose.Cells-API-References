---
title: Validation.Operator
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the operator for the data validation
type: docs
url: /net/aspose.cells/validation/operator/
---
## Validation.Operator property

Represents the operator for the data validation.

```csharp
public OperatorType Operator { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(valSrc.Operator, valDest.Operator, info + ".Operator");
public static void Property_Operator(Validation valSrc, Validation valDest, string info)
        {
            if (AssertHelper.checkNull(valSrc, valDest, info))
            {
                return;
            }
            AssertHelper.equalsItems(valSrc.Areas, valDest.Areas, info + ".AreaList");

            //Settings
            AssertHelper.AreEqual(valSrc.Type, valDest.Type, info + ".Type");
            if (valSrc.Type != ValidationType.List)
            {
                AssertHelper.AreEqual(valSrc.Operator, valDest.Operator, info + ".Operator");
            }
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

* enum [OperatorType](../../operatortype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


