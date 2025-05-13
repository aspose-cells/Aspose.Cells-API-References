---
title: ImportTableOptions.IsHtmlString
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Indicates whether the value contains html tags
type: docs
url: /net/aspose.cells/importtableoptions/ishtmlstring/
---
## ImportTableOptions.IsHtmlString property

Indicates whether the value contains html tags.

```csharp
public bool IsHtmlString { get; set; }
```

### Examples

```csharp
// Called: IsHtmlString = true
public void ImportTableOptions_Property_IsHtmlString()
{
    System.Data.DataTable table = new System.Data.DataTable();
    table.Columns.Add("ID");
    table.Columns.Add("thelink");
    table.Columns.Add("Start Time");
    string[] addrow = { "1", "<span style='width: 240px; overflow: hidden; white-space: nowrap; display: inline-block; text-overflow:ellipsis;'><a href='http://mysite.com/includes/pdfcrowd/pdfAPI.php?url=https%3A%2F%2Fwww%2mysite%2Ecom%2Fcfp2%2FReviews%2FTools%2FPreview%2Dall%2Easp%3FEventID%3D9638%26ClientID%3D2465%26SubID%3D716990&pageheight=11in' target='_blank'>Submission Preview</a></span>", "1:00 PM" };
    table.Rows.Add(addrow);

    var workbook = new Workbook();
    var ws = workbook.Worksheets[0];
    ws.Cells.ImportData(table, 0, 0, new ImportTableOptions
    {
        IsFieldNameShown = true,
        ConvertNumericData = true,
        NumberFormats = new string[] { null, null, "h:mm AM/PM" },
        IsHtmlString = true


    });
    Hyperlink link = workbook.Worksheets[0].Hyperlinks[0];
    Assert.AreEqual(1, link.Area.StartRow);
    Assert.AreEqual(1, link.Area.StartColumn);
    workbook.Save(_destFilesPath + "example.xlsx");
}
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


