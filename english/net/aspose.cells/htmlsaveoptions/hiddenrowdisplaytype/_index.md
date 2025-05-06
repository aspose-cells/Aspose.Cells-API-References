---
title: HtmlSaveOptions.HiddenRowDisplayType
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Hidden rowthe height of this row is 0 in excelbefore save this into html format if HtmlHiddenRowDisplayType is Removethe hidden row would not been output if the value is Hidden the row would been outputbut was hiddenthe default value is Hidden
type: docs
url: /net/aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/
---
## HtmlSaveOptions.HiddenRowDisplayType property

Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden"

```csharp
public HtmlHiddenRowDisplayType HiddenRowDisplayType { get; set; }
```

### Examples

```csharp
// Called: HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove
[Test]
        public void Property_HiddenRowDisplayType()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET47261/&quot;;

            var workBook = new Workbook(filePath + &quot;Test2.xlsx&quot;);
            string RangeName = &quot;RANGE1&quot;;
            var range = Array.Find(workBook.Worksheets.GetNamedRanges(), r =&gt; r.Name == RangeName);

            var sheet = range.Worksheet;
            var cells = sheet.Cells;
            var firstCol = range.FirstColumn;
            var firstRow = range.FirstRow;
            var maxCol = cells.MaxDisplayRange.ColumnCount;
            var maxRow = cells.MaxDisplayRange.RowCount;

            if (firstCol &gt; 0)
            {
                cells.HideColumns(0, firstCol);
            }
            if (firstCol + range.ColumnCount &lt; maxCol)
            {
                cells.HideColumns(firstCol + range.ColumnCount, maxCol - (firstCol + range.ColumnCount));
            }
            if (firstRow &gt; 0)
            {
                cells.HideRows(0, firstRow);
            }
            if (firstRow + range.RowCount &lt; maxRow)
            {
                cells.HideRows(firstRow + range.RowCount, maxRow - (firstRow + range.RowCount));
            }

            range.Worksheet.Workbook.Worksheets.ActiveSheetIndex = sheet.Index;

            var opts = new HtmlSaveOptions()
            {
                Encoding = Encoding.UTF8,
                HtmlCrossStringType = HtmlCrossType.Cross,
                PresentationPreference = true,
                ExportHiddenWorksheet = false,
                ExportActiveWorksheetOnly = true,
                ExportImagesAsBase64 = true,
                CreateDirectory = false,
                IsExpImageToTempDir = false,
                HiddenColDisplayType = HtmlHiddenColDisplayType.Remove,
                HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove
            };
            range.Worksheet.Workbook.Save(CreateFolder(filePath) + &quot;out2.html&quot;, opts);

        }
```

### See Also

* enum [HtmlHiddenRowDisplayType](../../htmlhiddenrowdisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


