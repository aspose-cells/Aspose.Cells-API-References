---
title: GroupBox.Shadow
second_title: Aspose.Cells for .NET API Reference
description: GroupBox property. Indicates whether the groupbox has shadow
type: docs
url: /net/aspose.cells.drawing/groupbox/shadow/
---
## GroupBox.Shadow property

Indicates whether the groupbox has shadow.

```csharp
public bool Shadow { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(gboxSrc.Shadow, gboxDest.Shadow, info + ".Shadow");
public static void GroupBox_Property_Shadow(GroupBox gboxSrc, GroupBox gboxDest, string info)
        {
            if (AssertHelper.checkNull(gboxSrc, gboxDest, info))
            {
                return;
            }
            //================properties are supported in excel 2003 format=================//
            AssertHelper.AreEqual(gboxSrc.AutoShapeType, gboxDest.AutoShapeType, info + ".AutoShapeType");
            AssertHelper.AreEqual(gboxSrc.MsoDrawingType, gboxDest.MsoDrawingType, info + ".MsoDrawingType");           
            AssertHelper.AreEqual(gboxSrc.UpperLeftRow, gboxDest.UpperLeftRow, info + ".UpperLeftRow");
            AssertHelper.AreEqual(gboxSrc.UpperLeftColumn, gboxDest.UpperLeftColumn, info + ".UpperLeftColumn");
            AssertHelper.AreEqual(gboxSrc.LowerRightRow, gboxDest.LowerRightRow, info + ".LowerRightRow");
            AssertHelper.AreEqual(gboxSrc.LowerRightColumn, gboxDest.LowerRightColumn, info + ".LowerRightColumn");     
            //===size===//
            AssertHelper.AreEqual(gboxSrc.HeightCM, gboxDest.HeightCM, info + ".HeightCM");
            AssertHelper.AreEqual(gboxSrc.WidthCM, gboxDest.WidthCM, info + ".WidthCM");
            AssertHelper.AreEqual(gboxSrc.HeightScale, gboxDest.HeightScale, info + ".HeightScale");
            AssertHelper.AreEqual(gboxSrc.WidthScale, gboxDest.WidthScale, info + ".WidthScale");
            AssertHelper.AreEqual(gboxSrc.IsLockAspectRatio, gboxDest.IsLockAspectRatio, info + ".IsLockAspectRatio");
            //===protection===//
            AssertHelper.AreEqual(gboxSrc.IsLocked, gboxDest.IsLocked, info + ".IsLocked");
            //===properties===//
            AssertHelper.AreEqual(gboxSrc.Placement, gboxDest.Placement, info + ".Placement");
            AssertHelper.AreEqual(gboxSrc.IsPrintable, gboxDest.IsPrintable, info + ".IsPrintable");
            //===web===//
            AssertHelper.AreEqual(gboxSrc.AlternativeText, gboxDest.AlternativeText, info + ".AlternativeText");
            //===control===//
            AssertHelper.AreEqual(gboxSrc.Shadow, gboxDest.Shadow, info + ".Shadow");
            //other
            AssertHelper.AreEqual(gboxSrc.IsHidden, gboxDest.IsHidden, info + ".IsHidden");
            AssertHelper.AreEqual(gboxSrc.IsGroup, gboxDest.IsGroup, info + ".IsGroup");
        }
```

### See Also

* class [GroupBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


