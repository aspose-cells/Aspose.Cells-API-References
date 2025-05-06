---
title: CopyOptions.ReferToDestinationSheet
second_title: Aspose.Cells for .NET API Reference
description: CopyOptions property. When copying the range in the same file and the chart refers to the source sheet False means the copied charts data source will not be changed. True means the copied charts data source refers to the destination sheet
type: docs
url: /net/aspose.cells/copyoptions/refertodestinationsheet/
---
## CopyOptions.ReferToDestinationSheet property

When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet.

```csharp
public bool ReferToDestinationSheet { get; set; }
```

### Remarks

The default value is false, it works as MS Excel.

### Examples

```csharp
// Called: options.ReferToDestinationSheet = true;
[Test]
        public void Property_ReferToDestinationSheet()
        {
            var book = new Workbook(Constants.sourcePath + &quot;CellsNet44626.xlsx&quot;);
            var source = book.Worksheets[0];
            var destination = book.Worksheets[book.Worksheets.Add()];
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;

            destination.Cells.CopyRows(source.Cells, 0, 0, source.Cells.MaxDisplayRange.RowCount, options);
            Assert.AreEqual(destination.Charts[0].NSeries[0].Values, &quot;=Sheet2!$B$2:$B$4&quot;);
            Util.ReSave(book, SaveFormat.Xlsx);
            //book.Save(Constants.destPath + &quot;CellsNet44626.xlsx&quot;);
        }
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


