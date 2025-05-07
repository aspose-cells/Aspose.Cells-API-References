---
title: Range.Worksheet
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the Worksheetobject which contains this range
type: docs
url: /net/aspose.cells/range/worksheet/
---
## Range.Worksheet property

Gets the `Worksheet`object which contains this range.

```csharp
public Worksheet Worksheet { get; }
```

### Examples

```csharp
// Called: Worksheet ws = range.Worksheet;
[Test]
        public void Property_Worksheet()
        {
            Workbook wb = new Workbook(Constants.HtmlPath + "CELLSJAVA-45957.xlsx"); 
            Aspose.Cells.Range range = wb.Worksheets.GetRangeByName("PIANETI");
            Worksheet ws = range.Worksheet;
            PageSetup pageSetup = ws.PageSetup;
            pageSetup.PrintArea = (range.Address);
            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
            options.ExportPrintAreaOnly = true;
            options.ExportBogusRowData = false;
            wb.Save(_destFilesPath + "CELLSJAVA-45957.html", options);
            string text = File.ReadAllText(_destFilesPath + "CELLSJAVA-45957.html");
            Assert.IsTrue(text.IndexOf("font-family:Pacifico,sans-serif;") > -1);
            options.AddGenericFont = false;
            wb.Save(_destFilesPath + "CELLSJAVA-45957.html", options);
            text = File.ReadAllText(_destFilesPath + "CELLSJAVA-45957.html");
            Assert.IsTrue(text.IndexOf("font-family:Pacifico,sans-serif;") == -1);
        }
```

### See Also

* class [Worksheet](../../worksheet/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


