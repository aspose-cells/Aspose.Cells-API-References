---
title: InsertOptions.CopyFormatType
second_title: Aspose.Cells for .NET API Reference
description: InsertOptions property. 
type: docs
url: /net/aspose.cells/insertoptions/copyformattype/
---
## InsertOptions.CopyFormatType property

```csharp
public CopyFormatType CopyFormatType { get; set; }
```

### Examples

```csharp
// Called: cells.InsertRows(1, 1, new InsertOptions() { CopyFormatType = CopyFormatType.Clear });
[Test]
        public void Property_CopyFormatType()
        {
            Workbook workbook = new Workbook();

            Cells cells = workbook.Worksheets[0].Cells;
            cells.InsertRows(0, 1);

            var style = workbook.CreateStyle();
            var flag = new StyleFlag();

            style.Font.IsBold = true;
            flag.FontBold = true;

            cells.Rows[0].ApplyStyle(style, flag);
            cells[0, 0].PutValue("First Row we Created");//row, col
            cells.InsertRows(1, 1, new InsertOptions() { CopyFormatType = CopyFormatType.Clear });
            cells[1, 0].PutValue("Second Row we Created");// THIS TEXT SHOULD NOT BE BOLD AS CLEAR IS USED ABOVE
            Assert.IsFalse(workbook.Worksheets[0].Cells[1, 0].GetStyle().Font.IsBold);

            workbook.Save(Constants.destPath + "CELLSNET46609.xlsx");
        }
```

### See Also

* enum [CopyFormatType](../../copyformattype/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


