---
title: Style.ShrinkToFit
second_title: Aspose.Cells for .NET API Reference
description: Style property. Represents if text automatically shrinks to fit in the available column width
type: docs
url: /net/aspose.cells/style/shrinktofit/
---
## Style.ShrinkToFit property

Represents if text automatically shrinks to fit in the available column width.

```csharp
public bool ShrinkToFit { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(styleSrc.ShrinkToFit, styleDest.ShrinkToFit, info + ".ShrinkToFit");
public static void Property_ShrinkToFit(Style styleSrc, Style styleDest, string info)
        {
            AssertHelper.AreEqual(styleSrc.HorizontalAlignment, styleDest.HorizontalAlignment, info + ".HorizontalAlignment");
            AssertHelper.AreEqual(styleSrc.VerticalAlignment, styleDest.VerticalAlignment, info + ".VerticalAlignment");
            AssertHelper.AreEqual(styleSrc.IndentLevel, styleDest.IndentLevel, info + ".IndentLevel");
            AssertHelper.AreEqual(styleSrc.IsTextWrapped, styleDest.IsTextWrapped, info + ".IsTextWrapped");
            AssertHelper.AreEqual(styleSrc.ShrinkToFit, styleDest.ShrinkToFit, info + ".ShrinkToFit");
            AssertHelper.AreEqual(styleSrc.TextDirection, styleDest.TextDirection, info + ".TextDirection");
            AssertHelper.AreEqual(styleSrc.RotationAngle, styleDest.RotationAngle, info + ".Rotation");
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


