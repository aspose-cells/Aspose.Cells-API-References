---
title: SaveOptions.CreateDirectory
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. If true and the directory does not exist the directory will be automatically created before saving the file
type: docs
url: /net/aspose.cells/saveoptions/createdirectory/
---
## SaveOptions.CreateDirectory property

If true and the directory does not exist, the directory will be automatically created before saving the file.

```csharp
public bool CreateDirectory { get; set; }
```

### Remarks

The default value is false.

### Examples

```csharp
// Called: saveOps.CreateDirectory = false;
[Test]
        public void Property_CreateDirectory()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42277/";

            String fileName = "PusheenVisio-20170427.xlsx";

            Workbook book = new Workbook(filePath + fileName);

            book.Worksheets["工作表2"].IsVisible = false;
            book.Worksheets["工作表3"].IsVisible = false;

            HtmlSaveOptions saveOps = new HtmlSaveOptions();
            saveOps.ClearData = false;
            saveOps.CreateDirectory = false;
            saveOps.ExportActiveWorksheetOnly = false;
            saveOps.ExportHiddenWorksheet = false;
            ; //Comment this line and image will display fine
            saveOps.ParseHtmlTagInCell = true;
            saveOps.Encoding = Encoding.UTF8;
            saveOps.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove;
            saveOps.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;
            saveOps.ExportImagesAsBase64 = true;
            book.Save(_destFilesPath + "JAVA42277.html", saveOps);
            book = new Workbook(_destFilesPath + "JAVA42277.html");
            Assert.AreEqual(book.Worksheets.Count, 1);
            Assert.AreEqual(book.Worksheets[0].Shapes.Count, 2);
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


