---
title: LoadOptions.Region
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets or sets the system regional settings based on CountryCode at the time the file was loaded
type: docs
url: /net/aspose.cells/loadoptions/region/
---
## LoadOptions.Region property

Gets or sets the system regional settings based on CountryCode at the time the file was loaded.

```csharp
public CountryCode Region { get; set; }
```

### Remarks

If you do not want to use the region saved in the file, please reset it after reading the file.

### Examples

```csharp
// Called: loadOpts.Region = CountryCode.USA;
public void LoadOptions_Property_Region()
{
    LoadOptions loadOpts = new LoadOptions(LoadFormat.Html);
    loadOpts.Region = CountryCode.USA;
    Workbook wb = new Workbook(Constants.HtmlPath + "example.html", loadOpts);
    Worksheet ws = wb.Worksheets[0];
    for (int i = 0; i < ws.Hyperlinks.Count; i++)
    {
        Hyperlink hyperlink = ws.Hyperlinks[i];
        hyperlink.Delete();
    }
    Aspose.Cells.Font font = ws.Cells["A14"].GetStyle().Font;
    Assert.AreEqual("Arial", font.Name);
    Assert.AreEqual(10, font.Size);
    Assert.IsFalse(font.IsItalic);
    CompareColor.compare("A14", Color.FromArgb(255, 0, 0, 0), font.Color);
}
```

### See Also

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


