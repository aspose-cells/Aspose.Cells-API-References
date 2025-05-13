---
title: ReplaceOptions.CaseSensitive
second_title: Aspose.Cells for .NET API Reference
description: ReplaceOptions property. Indicates if the searched string is case sensitive
type: docs
url: /net/aspose.cells/replaceoptions/casesensitive/
---
## ReplaceOptions.CaseSensitive property

Indicates if the searched string is case sensitive.

```csharp
public bool CaseSensitive { get; set; }
```

### Examples

```csharp
// Called: TempExcelReplaceOptions.CaseSensitive = false;
public void ReplaceOptions_Property_CaseSensitive()
{
    Aspose.Cells.Workbook TempExcelDocument = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xlsx");
    Console.WriteLine(TempExcelDocument.Worksheets[0].Cells["A1"].StringValue);
    Aspose.Cells.ReplaceOptions TempExcelReplaceOptions = new Aspose.Cells.ReplaceOptions();
    Aspose.Cells.OoxmlSaveOptions TempXlsxSaveOption = new OoxmlSaveOptions();
    TempExcelReplaceOptions.MatchEntireCellContents = false;
    TempExcelReplaceOptions.CaseSensitive = false;
    TempExcelReplaceOptions.RegexKey = false;
    TempExcelDocument.Replace("2/2024", "3/2025", TempExcelReplaceOptions);

   Assert.AreEqual("1/3/2025", TempExcelDocument.Worksheets[0].Cells["A2"].StringValue);
}
```

### See Also

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


