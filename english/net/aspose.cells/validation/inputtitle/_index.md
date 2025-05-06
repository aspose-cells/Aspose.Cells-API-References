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
// Called: AssertHelper.AreEqual(valSrc.InputTitle, valDest.InputTitle, info + &amp;quot;.InputTitle&amp;quot;);
public static void Property_InputTitle(Validation valSrc, Validation valDest, string info)
        {
            if (AssertHelper.checkNull(valSrc, valDest, info))
            {
                return;
            }
            AssertHelper.equalsItems(valSrc.Areas, valDest.Areas, info + &quot;.AreaList&quot;);

            //Settings
            AssertHelper.AreEqual(valSrc.Type, valDest.Type, info + &quot;.Type&quot;);
            if (valSrc.Type != ValidationType.List)
            {
                AssertHelper.AreEqual(valSrc.Operator, valDest.Operator, info + &quot;.Operator&quot;);
            }
            AssertHelper.AreEqual(valSrc.IgnoreBlank, valDest.IgnoreBlank, info + &quot;.IgnoreBlank&quot;);
            AssertHelper.AreEqual(valSrc.InCellDropDown, valDest.InCellDropDown, info + &quot;.InCellDropDown&quot;);
            AssertHelper.AreEqual(valSrc.Formula1, valDest.Formula1, info + &quot;.Formula1&quot;);
            AssertHelper.AreEqual(valSrc.Formula2, valDest.Formula2, info + &quot;.Formula2&quot;);
            //Input message
            AssertHelper.AreEqual(valSrc.InputTitle, valDest.InputTitle, info + &quot;.InputTitle&quot;);
            AssertHelper.AreEqual(valSrc.InputMessage, valDest.InputMessage, info + &quot;.InputMessage&quot;);
            //Error alert
            AssertHelper.AreEqual(valSrc.AlertStyle, valDest.AlertStyle, info + &quot;.AlertStyle&quot;);
            AssertHelper.AreEqual(valSrc.ErrorTitle, valDest.ErrorTitle, info + &quot;.ErrorTitle&quot;);
            AssertHelper.AreEqual(valSrc.ErrorMessage, valDest.ErrorMessage, info + &quot;.ErrorMessage&quot;);
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


