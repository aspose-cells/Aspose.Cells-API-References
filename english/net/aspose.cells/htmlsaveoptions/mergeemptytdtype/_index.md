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
[Test]
        public void Property_MergeEmptyTdType()
        {
            Workbook workbook = new Workbook(Constants.HtmlPath + "CELLSJAVA-46332.xlsx");
            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html)
            {
                ExportPrintAreaOnly = true,
                ExportActiveWorksheetOnly = true,
                AddGenericFont = false,
                ExportBogusRowData = false,
                HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove,
                HiddenColDisplayType = HtmlHiddenColDisplayType.Remove,
                MergeEmptyTdType = MergeEmptyTdType.None,
            };
            WorksheetCollection worksheets = workbook.Worksheets;
            string rangeName = "All 5 columns tables!SUMMARY";
            Aspose.Cells.Range range = worksheets.GetRangeByName(rangeName);
            workbook.Worksheets.ActiveSheetIndex = range.Worksheet.Index;
            range.Worksheet.PageSetup.PrintArea = range.Address;
            workbook.Save(_destFilesPath + "CELLSJAVA-46332.html", options);
            string text = File.ReadAllText(_destFilesPath + "CELLSJAVA-46332.html");
            Regex reg = new Regex(">Twelve months ended</td>\\s*<td[^>]*></td>\\s*</tr>");
            Assert.IsTrue(reg.IsMatch(text));
        }
```

### See Also

* enum [MergeEmptyTdType](../../mergeemptytdtype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


