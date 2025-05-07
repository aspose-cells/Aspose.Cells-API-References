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
// Called: cells.SetColumnWidthPixel(i, 100);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Aspose.Cells.Style defaultStyle = workbook.DefaultStyle;
            defaultStyle.Font.Name = "Tahoma";
            defaultStyle.Font.Size = 14;
            defaultStyle.Font.IsBold = true;
            workbook.DefaultStyle = defaultStyle;
            Cells cells = workbook.Worksheets[0].Cells;

            for (int i = 1; i < 16; i++)
                cells.SetColumnWidthPixel(i, 100);
            workbook.Save(Constants.destPath + "Test_146652.xls");
            workbook = new Workbook(Constants.destPath + "Test_146652.xls");
            Assert.AreEqual(workbook.Worksheets[0].Cells.GetColumnWidthPixel(1), 100);

        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


