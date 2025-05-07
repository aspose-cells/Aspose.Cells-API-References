---
title: Floor.Border
second_title: Aspose.Cells for .NET API Reference
description: Floor property. Gets or sets the border Line
type: docs
url: /net/aspose.cells.charts/floor/border/
---
## Floor.Border property

Gets or sets the border [`Line`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; set; }
```

### Examples

```csharp
// Called: LineTest.equals(wallsSrc.Border, wallsDest.Border, info+".Border");
public static void Property_Border(Walls wallsSrc, Walls wallsDest, string info)
        {
            if (AssertHelper.checkNull(wallsSrc, wallsDest, info))
            {
                return;
            }
            //============compare patterns====================//
            LineTest.Property_Border(wallsSrc.Border, wallsDest.Border, info+".Border");
            AssertHelper.AreEqual(wallsSrc.Formatting, wallsDest.Formatting, info + ".Formatting");
            if (wallsSrc.Formatting == FormattingType.Custom)
            {
                FillFormatTest.Property_Border(wallsSrc.FillFormat, wallsDest.FillFormat, info+".FillFormat");
                AssertHelper.Property_Border(wallsSrc.ForegroundColor, wallsDest.ForegroundColor, info + ".ForegroundColor");
                AssertHelper.Property_Border(wallsSrc.BackgroundColor, wallsDest.BackgroundColor, info + ".BackgroundColor");                
            }

            AssertHelper.AreEqual(wallsSrc.Transparency, wallsDest.Transparency, info + ".Transparency");
            AssertHelper.AreEqual(wallsSrc.InvertIfNegative, wallsDest.InvertIfNegative, info + ".InvertIfNegative");
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [Floor](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


