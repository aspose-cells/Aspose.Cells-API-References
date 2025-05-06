---
title: ComboBox.DropDownLines
second_title: Aspose.Cells for .NET API Reference
description: ComboBox property. Gets or sets the number of list lines displayed in the dropdown portion of a combo box
type: docs
url: /net/aspose.cells.drawing/combobox/dropdownlines/
---
## ComboBox.DropDownLines property

Gets or sets the number of list lines displayed in the drop-down portion of a combo box.

```csharp
public int DropDownLines { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cboxSrc.DropDownLines, cboxDest.DropDownLines, info + &amp;quot;.DropDownLines&amp;quot;);
public static void Property_DropDownLines(ComboBox cboxSrc, ComboBox cboxDest, string info)
        {
            if (AssertHelper.checkNull(cboxSrc, cboxDest, info))
            {
                return;
            }
            //========================need be supported in excel 2003 format=======================//
            AssertHelper.AreEqual(cboxSrc.MsoDrawingType, cboxDest.MsoDrawingType, info + &quot;.MsoDrawingType&quot;);
            AssertHelper.AreEqual(cboxSrc.UpperLeftRow, cboxDest.UpperLeftRow, info + &quot;.UpperLeftRow&quot;);
            AssertHelper.AreEqual(cboxSrc.UpperLeftColumn, cboxDest.UpperLeftColumn, info + &quot;.UpperLeftColumn&quot;);
            AssertHelper.AreEqual(cboxSrc.LowerRightRow, cboxDest.LowerRightRow, info + &quot;.LowerRightRow&quot;);
            AssertHelper.AreEqual(cboxSrc.LowerRightColumn, cboxDest.LowerRightColumn, info + &quot;.LowerRightColumn&quot;);     
            //size
            AssertHelper.AreEqual(cboxSrc.Height, cboxDest.Height, info+&quot;.Height&quot;);
            AssertHelper.AreEqual(cboxSrc.Width, cboxDest.Width, info+&quot;.Width&quot;);
            AssertHelper.AreEqual(cboxSrc.HeightScale, cboxDest.HeightScale, info + &quot;.HeightScale&quot;);
            AssertHelper.AreEqual(cboxSrc.WidthScale, cboxDest.WidthScale, info + &quot;.WidthScale&quot;);
            AssertHelper.AreEqual(cboxSrc.IsLockAspectRatio, cboxDest.IsLockAspectRatio, info+&quot;.IsLockAspectRatio&quot;);
            //protection
            AssertHelper.AreEqual(cboxSrc.IsLocked, cboxDest.IsLocked, info + &quot;.IsLocked&quot;);
            //properties
            AssertHelper.AreEqual(cboxSrc.Placement, cboxDest.Placement, info + &quot;.Placement&quot;);
            AssertHelper.AreEqual(cboxSrc.IsPrintable, cboxDest.IsPrintable, info + &quot;.IsPrintable&quot;);
            //web
            AssertHelper.AreEqual(cboxSrc.AlternativeText, cboxDest.AlternativeText, info + &quot;.AlternativeText&quot;);
            //control
            AssertHelper.AreEqual(cboxSrc.InputRange, cboxDest.InputRange, info + &quot;.InputRange&quot;);
            AssertHelper.AreEqual(cboxSrc.LinkedCell, cboxDest.LinkedCell, info + &quot;.LinkedCell&quot;);
            AssertHelper.AreEqual(cboxSrc.DropDownLines, cboxDest.DropDownLines, info + &quot;.DropDownLines&quot;);
            AssertHelper.AreEqual(cboxSrc.Shadow, cboxDest.Shadow, info + &quot;.Shadow&quot;);
            //other
            AssertHelper.AreEqual(cboxSrc.IsHidden, cboxDest.IsHidden, info + &quot;.IsHidden&quot;);
            AssertHelper.AreEqual(cboxSrc.IsGroup, cboxDest.IsGroup, info + &quot;.IsGroup&quot;);
        }
```

### See Also

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


