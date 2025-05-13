---
title: HtmlSaveOptions.PresentationPreference
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentationplease set the value to true
type: docs
url: /net/aspose.cells/htmlsaveoptions/presentationpreference/
---
## HtmlSaveOptions.PresentationPreference property

Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true.

```csharp
public bool PresentationPreference { get; set; }
```

### Examples

```csharp
// Called: options.PresentationPreference = true;
public void HtmlSaveOptions_Property_PresentationPreference()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA43533/";
    string savePath = CreateFolder(filePath);

    Workbook workbook = new Workbook(filePath + "TestAspose.xlsx");
    HtmlSaveOptions options = new HtmlSaveOptions();
    options.PresentationPreference = true;
    options.IsFullPathLink = true;
    options.StreamProvider = new ExportStreamProvider(savePath + @"output\");

    FileStream outStream = new FileStream(savePath + "out.html", FileMode.Create);
    workbook.Save(outStream, options);

}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


