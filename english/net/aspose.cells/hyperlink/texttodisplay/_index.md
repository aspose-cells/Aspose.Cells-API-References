---
title: Hyperlink.TextToDisplay
second_title: Aspose.Cells for .NET API Reference
description: Hyperlink property. Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink
type: docs
url: /net/aspose.cells/hyperlink/texttodisplay/
---
## Hyperlink.TextToDisplay property

Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink.

```csharp
public string TextToDisplay { get; set; }
```

### Examples

```csharp
// Called: hyperLinks[index].TextToDisplay = "A1:B6";
public void Hyperlink_Property_TextToDisplay()
{
    Workbook workbook = new Workbook();
    WorksheetCollection worksheets = workbook.Worksheets;
    Worksheet worksheet = worksheets[0];
    HyperlinkCollection hyperLinks = worksheet.Hyperlinks;
    int index = hyperLinks.Add("H2", 1, 1, "\\\\harsh\\File Share\\DEMO Files\\v1.21.xlsm#'Control'!A1:B6");
    hyperLinks[index].TextToDisplay = "A1:B6";

    index = hyperLinks.Add("H3", 1, 1, "E:\\VSCellsForm\\sample.xlsx#'Sheet1'!A1:B6");
    hyperLinks[index].TextToDisplay = "A1:B6";

    MemoryStream ms = Util.SaveAsBuffer(workbook, SaveFormat.Xlsx);
    Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(ms,
    //workbook.Save(Constants.destPath + "example.xlsx");
    //Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + @"example.xlsx",
        "xl/worksheets/_rels/sheet1.xml.rels", new string[] { "file:///\\\\harsh" }, true));
}
```

### See Also

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


