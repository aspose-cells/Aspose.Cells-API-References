---
title: ComboBox.Shadow
second_title: Aspose.Cells for .NET API Reference
description: ComboBox property. Indicates whether the combobox has 3D shading
type: docs
url: /net/aspose.cells.drawing/combobox/shadow/
---
## ComboBox.Shadow property

Indicates whether the combobox has 3-D shading.

```csharp
public bool Shadow { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cboxSrc.Shadow, cboxDest.Shadow, info + ".Shadow");
public static void Property_Shadow(ComboBox cboxSrc, ComboBox cboxDest, string info)
        {
            if (AssertHelper.checkNull(cboxSrc, cboxDest, info))
            {
                return;
            }
            //========================need be supported in excel 2003 format=======================//
            AssertHelper.AreEqual(cboxSrc.MsoDrawingType, cboxDest.MsoDrawingType, info + ".MsoDrawingType");
            AssertHelper.AreEqual(cboxSrc.UpperLeftRow, cboxDest.UpperLeftRow, info + ".UpperLeftRow");
            AssertHelper.AreEqual(cboxSrc.UpperLeftColumn, cboxDest.UpperLeftColumn, info + ".UpperLeftColumn");
            AssertHelper.AreEqual(cboxSrc.LowerRightRow, cboxDest.LowerRightRow, info + ".LowerRightRow");
            AssertHelper.AreEqual(cboxSrc.LowerRightColumn, cboxDest.LowerRightColumn, info + ".LowerRightColumn");     
            //size
            AssertHelper.AreEqual(cboxSrc.Height, cboxDest.Height, info+".Height");
            AssertHelper.AreEqual(cboxSrc.Width, cboxDest.Width, info+".Width");
            AssertHelper.AreEqual(cboxSrc.HeightScale, cboxDest.HeightScale, info + ".HeightScale");
            AssertHelper.AreEqual(cboxSrc.WidthScale, cboxDest.WidthScale, info + ".WidthScale");
            AssertHelper.AreEqual(cboxSrc.IsLockAspectRatio, cboxDest.IsLockAspectRatio, info+".IsLockAspectRatio");
            //protection
            AssertHelper.AreEqual(cboxSrc.IsLocked, cboxDest.IsLocked, info + ".IsLocked");
            //properties
            AssertHelper.AreEqual(cboxSrc.Placement, cboxDest.Placement, info + ".Placement");
            AssertHelper.AreEqual(cboxSrc.IsPrintable, cboxDest.IsPrintable, info + ".IsPrintable");
            //web
            AssertHelper.AreEqual(cboxSrc.AlternativeText, cboxDest.AlternativeText, info + ".AlternativeText");
            //control
            AssertHelper.AreEqual(cboxSrc.InputRange, cboxDest.InputRange, info + ".InputRange");
            AssertHelper.AreEqual(cboxSrc.LinkedCell, cboxDest.LinkedCell, info + ".LinkedCell");
            AssertHelper.AreEqual(cboxSrc.DropDownLines, cboxDest.DropDownLines, info + ".DropDownLines");
            AssertHelper.AreEqual(cboxSrc.Shadow, cboxDest.Shadow, info + ".Shadow");
            //other
            AssertHelper.AreEqual(cboxSrc.IsHidden, cboxDest.IsHidden, info + ".IsHidden");
            AssertHelper.AreEqual(cboxSrc.IsGroup, cboxDest.IsGroup, info + ".IsGroup");
        }
```

### See Also

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


