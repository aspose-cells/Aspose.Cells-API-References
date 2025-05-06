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
// Called: options.ExcludeUnusedStyles = true;
[Test]
        public void Property_ExcludeUnusedStyles()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA43162/&quot;;

            Workbook workbook = new Workbook(filePath + &quot;878914550142091892.xls&quot;);
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportDocumentProperties = false;
            options.ExportWorkbookProperties = false;
            options.ExportWorkbookProperties = false;
            options.ExportSimilarBorderStyle = true;
            options.ExportImagesAsBase64 = false;
            options.ExcludeUnusedStyles = true;
            options.ExportHiddenWorksheet = false;
            options.WidthScalable = false;
            options.PresentationPreference = true;
            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;


            workbook.Save(CreateFolder(filePath) + &quot;out.html&quot;);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


