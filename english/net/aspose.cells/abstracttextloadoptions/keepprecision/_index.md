---
title: AbstractTextLoadOptions.KeepPrecision
second_title: Aspose.Cells for .NET API Reference
description: AbstractTextLoadOptions property. Indicates whether not parsing a string value if the length is 15
type: docs
url: /net/aspose.cells/abstracttextloadoptions/keepprecision/
---
## AbstractTextLoadOptions.KeepPrecision property

Indicates whether not parsing a string value if the length is 15.

```csharp
public bool KeepPrecision { get; set; }
```

### Examples

```csharp
// Called: loadOptions.KeepPrecision = true;
public void AbstractTextLoadOptions_Property_KeepPrecision()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET45182/";

    HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
    loadOptions.SupportDivTag = true;
    loadOptions.KeepPrecision = true;
    loadOptions.AutoFitColsAndRows = true;
    Workbook wb = new Workbook(filePath + "input.html", loadOptions);
    //Assert.AreEqual(wb.Worksheets[0].Cells.MergedCells.Count, 695);
    var worksheet = wb.Worksheets[0];
    for (int i = 0; i < worksheet.Pictures.Count; i++)
    {
        Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[i];
        pic.Height = 250;
        pic.Width = 300;
        worksheet.Cells.SetRowHeight(pic.UpperLeftRow, 200);
    }

    wb.Save(CreateFolder(filePath) + "out.xlsx", Aspose.Cells.SaveFormat.Xlsx);
}
```

### See Also

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


