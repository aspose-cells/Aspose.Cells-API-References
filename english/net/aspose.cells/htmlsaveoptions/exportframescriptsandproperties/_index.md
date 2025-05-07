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
// Called: ExportFrameScriptsAndProperties = false,
[Test]
        public void Property_ExportFrameScriptsAndProperties()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET44446/";
            var wb = new Workbook(filePath + @"Blank.xlsx");
            var cells = wb.Worksheets[0].Cells;
            var wsUniqueId = new Random().Next(0, UInt16.MaxValue);
            int firstRow = 0, firstColumn = 0;

            var hso = new HtmlSaveOptions(SaveFormat.Html)
            {
                CellCssPrefix = "Shakeel" + wsUniqueId + cells[firstRow, firstColumn].Name,
                ExportActiveWorksheetOnly = true,
                ExportDataOptions = HtmlExportDataOptions.All,
                ExportFrameScriptsAndProperties = false,
                ExportImagesAsBase64 = true,
                HiddenColDisplayType = HtmlHiddenColDisplayType.Remove,
                HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove,
                HtmlCrossStringType = HtmlCrossType.Default,
            };
            wb.Save(CreateFolder(filePath) + "out.html", hso);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


