---
title: HtmlSaveOptions.MergeEmptyTdType
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. The option to merge contiguous empty cellsempty td elements The default value is MergeEmptyTdType.Default
type: docs
url: /net/aspose.cells/htmlsaveoptions/mergeemptytdtype/
---
## HtmlSaveOptions.MergeEmptyTdType property

The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default.

```csharp
public MergeEmptyTdType MergeEmptyTdType { get; set; }
```

### Examples

```csharp
// Called: MergeEmptyTdType = MergeEmptyTdType.None,
public void HtmlSaveOptions_Property_MergeEmptyTdType()
{
    Workbook workbook = new Workbook(Constants.HtmlPath + "example.xlsx");
    WorksheetCollection worksheets = workbook.Worksheets;
    string fullRangeName = $"Sheet1!TEST_AREA";
    Aspose.Cells.Range range = worksheets.GetRangeByName(fullRangeName);

    if (range == null && fullRangeName.Contains("!"))
    {
        string fallbackName = fullRangeName.Split('!')[1];
        range = worksheets.GetRangeByName(fallbackName);
    } 
    for (int r = 0; r < range.RowCount; r++)
    {
        for (int c = 0; c < range.ColumnCount; c++)
        {
            var cell = range[r, c];
            if (string.IsNullOrEmpty(cell.StringValue))
            {
                Style style = cell.GetStyle();
                style.ShrinkToFit = true;
                cell.SetStyle(style);
            }
        }
    }

    worksheets.ActiveSheetIndex = range.Worksheet.Index;
    range.Worksheet.PageSetup.PrintArea = range.Address;

    var htmlOptions = new HtmlSaveOptions(SaveFormat.Html)
    {
        ExportPrintAreaOnly = true,
        ExportActiveWorksheetOnly = true,
        AddGenericFont = false,
        ExportBogusRowData = false,
        HiddenColDisplayType = HtmlHiddenColDisplayType.Remove,
        HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove,
        MergeEmptyTdType = MergeEmptyTdType.None,
        CellNameAttribute = "id",
    };


    workbook.Save(_destFilesPath+ "example.html", htmlOptions);
    string text = File.ReadAllText(_destFilesPath + "example.html");
    Assert.IsTrue(text.IndexOf("<td id='I3' class='x44'>ABC</td>\n </tr>") > -1);


}
```

### See Also

* enum [MergeEmptyTdType](../../mergeemptytdtype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


