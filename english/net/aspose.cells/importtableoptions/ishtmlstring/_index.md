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
[Test]
        public void Property_IsHtmlString()
        {
            DataTable table = new DataTable();
            table.Columns.Add("ID");
            table.Columns.Add("thelink");
            table.Columns.Add("Start Time");
            string[] addrow = { "1", "<p><a href=\"https://reactjs.org/blog/2018/09/10/introducing-the-react-profiler.html\">CN Risk 3</a>&nbsp;</p>", "1:00 PM" };
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
            Assert.AreEqual(ws.Hyperlinks.Count, 1);
            workbook.Save(Constants.destPath + "CELLSNET50380.xlsx");

        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


