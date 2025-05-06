---
title: Cells.SetColumnWidthPixel
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Sets column width in unit of pixels in normal view
type: docs
url: /net/aspose.cells/cells/setcolumnwidthpixel/
---
## Cells.SetColumnWidthPixel method

Sets column width in unit of pixels in normal view.

```csharp
public void SetColumnWidthPixel(int column, int pixels)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |
| pixels | Int32 | Number of pixels. |

### Examples

```csharp
// Called: cells1.SetColumnWidthPixel(1, 80);
[Test]
        public void Method_Int32_()
        {
            //=============Write=======================//
            Workbook workbook1 = new Workbook();
            Style defaultstyle = workbook1.DefaultStyle;
            defaultstyle.Font.Name = &quot;Tahoma&quot;;
            defaultstyle.Font.Size = 16;
            defaultstyle.Font.IsBold = true;
            workbook1.DefaultStyle = defaultstyle;
            Cells cells1 = workbook1.Worksheets[0].Cells;
            cells1.SetColumnWidthPixel(0, 20);
            cells1.SetColumnWidthPixel(1, 80);
            int i;
            // Column widths
            for (i = 2; i &lt; 13; i++)
            {
                cells1.SetColumnWidthPixel(i, 64);
            }
            cells1.SetColumnWidthPixel(i, 512);
            cells1.SetColumnWidthPixel(i + 1, 20);
            //Row heights
            cells1.SetRowHeightPixel(i, 12);
            for (i = 37; i &lt; 128; i++)
                cells1.SetRowHeightPixel(i, 15);
            workbook1.Save(Constants.destPath + &quot;SetRowHeightPixel.xls&quot;);
            //=================Read================//
            Workbook workbook2 = new Workbook(Constants.destPath + &quot;SetRowHeightPixel.xls&quot;);
            Cells cells2 = workbook2.Worksheets[0].Cells;
            int j;
            // Column widths
            for (j = 2; j &lt; 13; j++)
            {
                Assert.AreEqual(64, cells2.GetColumnWidthPixel(j));
            }
            Assert.AreEqual(512, cells2.GetColumnWidthPixel(j));
            Assert.AreEqual(20, cells2.GetColumnWidthPixel(j + 1));
            //Rows heights
            Assert.AreEqual(12, cells2.GetRowHeightPixel(j));
            for (j = 37; j &lt; 128; j++)
            {
                Assert.AreEqual(15, cells2.GetRowHeightPixel(j));
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


