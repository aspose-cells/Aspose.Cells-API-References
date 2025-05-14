---
title: HtmlSaveOptions.ExcludeUnusedStyles
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether excludes unused styles. For the generated html files excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated htmlsuch as the scenario that user needs to restore the workbook from the generated html later please set this property as false
type: docs
url: /net/aspose.cells/htmlsaveoptions/excludeunusedstyles/
---
## HtmlSaveOptions.ExcludeUnusedStyles property

Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false.

```csharp
public bool ExcludeUnusedStyles { get; set; }
```

### Examples

```csharp
// Called: htmlSaveOptions.ExcludeUnusedStyles = true;
public void HtmlSaveOptions_Property_ExcludeUnusedStyles()
{
    Workbook wb = new Workbook();
    Cell cell = wb.Worksheets[0].Cells["A1"];
    cell.Value = "rich text with color";
    FontSetting fontSetting = new FontSetting(1, 7, wb.Worksheets);
    fontSetting.Font.Color = Color.Red;
    cell.SetCharacters(new FontSetting[] { fontSetting });

    cell = wb.Worksheets[0].Cells["A2"];
    cell.Value = "different font";
    Style style = cell.GetStyle();
    style.Font.Name = "Times New Roman";
    style.Font.Size = 24;
    cell.SetStyle(style);

    HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
    htmlSaveOptions.ExcludeUnusedStyles = true;

    string savePath = _destFilesPath + "example.html";
    wb.Save(savePath, htmlSaveOptions);

    string content = File.ReadAllText(savePath);
    Assert.IsTrue(content.IndexOf(".font0") > -1);
    Assert.IsTrue(content.IndexOf(".font2") > -1);
    Assert.IsTrue(content.IndexOf(".font1") == -1);

}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


