---
title: Worksheet.Index
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the index of sheet in the worksheet collection
type: docs
url: /net/aspose.cells/worksheet/index/
---
## Worksheet.Index property

Gets the index of sheet in the worksheet collection.

```csharp
public int Index { get; }
```

### Examples

```csharp
// Called: workbook.Worksheets.ActiveSheetIndex = rangeByName.Worksheet.Index;
[Test]
        public void Property_Index()
        {
            Workbook workbook = new Workbook(Constants.HtmlPath + "CELLSJAVA-46213.xlsx");
          
            WorksheetCollection worksheets = workbook.Worksheets;
            Aspose.Cells.Range rangeByName = worksheets.GetRangeByName("AREA");
            workbook.Worksheets.ActiveSheetIndex = rangeByName.Worksheet.Index;
            rangeByName.Worksheet.PageSetup.PrintArea = rangeByName.Address;
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportPrintAreaOnly = true;
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove;
            workbook.Save(_destFilesPath + "CELLSJAVA-46213.html", saveOptions);
            string text = File.ReadAllText(workbook.FileName);
            int count = 0;
            string tag = "<col";

            int index = 0;
            while ((index = text.IndexOf(tag, index)) != -1)
            {
                count++;
                index += tag.Length; // Move past the current <col> tag
            }
            Assert.AreEqual(4, count, "Col Count");
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


