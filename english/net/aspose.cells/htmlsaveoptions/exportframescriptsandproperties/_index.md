---
title: HtmlSaveOptions.ExportFrameScriptsAndProperties
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportframescriptsandproperties/
---
## HtmlSaveOptions.ExportFrameScriptsAndProperties property

Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```csharp
public bool ExportFrameScriptsAndProperties { get; set; }
```

### Examples

```csharp
// Called: htmlSaveOptions.ExportFrameScriptsAndProperties = false;
[Test]
        public void Property_ExportFrameScriptsAndProperties()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA42853/&quot;;

            Workbook workbook = new Workbook(filePath + &quot;view_qldtl_Admin.xlsx&quot;);
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            htmlSaveOptions.DisableDownlevelRevealedComments = true;
            htmlSaveOptions.ExcludeUnusedStyles = true;
            htmlSaveOptions.ExportActiveWorksheetOnly = true;
            htmlSaveOptions.ExportDocumentProperties = false;
            htmlSaveOptions.ExportFrameScriptsAndProperties = false;
            htmlSaveOptions.ExportImagesAsBase64 = false;
            htmlSaveOptions.ExportPrintAreaOnly = true;
            htmlSaveOptions.ExportSimilarBorderStyle = true;
            htmlSaveOptions.ExportWorkbookProperties = false;
            htmlSaveOptions.ExportWorksheetCSSSeparately = false;
            htmlSaveOptions.ExportWorksheetProperties = false;
            htmlSaveOptions.ParseHtmlTagInCell = true;
            htmlSaveOptions.HtmlCrossStringType = HtmlCrossType.FitToCell;

            DateTime start = DateTime.Now;

            workbook.Save(CreateFolder(filePath) + &quot;out.html&quot;, htmlSaveOptions);

            Assert.Less(DateTime.Now.Subtract(start).Seconds, 30);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


