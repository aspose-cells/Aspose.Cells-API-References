---
title: Worksheet.ClearComments
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Clears all comments in designer spreadsheet
type: docs
url: /net/aspose.cells/worksheet/clearcomments/
---
## Worksheet.ClearComments method

Clears all comments in designer spreadsheet.

```csharp
public void ClearComments()
```

### Examples

```csharp
// Called: _worksheet.ClearComments();
[Test]
        public void Method_ClearComments()
        {
           

            Aspose.Cells.LoadOptions loadOptions = new Aspose.Cells.LoadOptions(LoadFormat.Xlsx);
            loadOptions.CheckExcelRestriction = false;
            Aspose.Cells.Workbook document = new Workbook(Constants.sourcePath + "NET47544.xlsx", loadOptions);

            Worksheet worksheet = document.Worksheets[0];

            worksheet.IsSelected = true;
            worksheet.Workbook.Worksheets.ActiveSheetIndex = 0;
            worksheet.PageSetup.PrintArea = "A1:Z40";

            foreach (Worksheet _worksheet in document.Worksheets)
            {
                _worksheet.ClearComments();
                _worksheet.PageSetup.ClearHeaderFooter();
            }

            worksheet.Workbook.Save(_destFilesPath + "NET47544.html", SaveFormat.Html);
            string text = File.ReadAllText(_destFilesPath + "NET47544.html");
            Assert.IsTrue(text.IndexOf("z-index:13;margin-left:7px;margin-top:15px;width:128px;height:67px'>") != -1);
            worksheet.Workbook.Save(_destFilesPath + "NET47544.pdf", SaveFormat.Pdf);

            SheetRender sheetRendererToPng = new SheetRender(worksheet, GetSaveOptionsForPng());
            Console.WriteLine("pageScale " + sheetRendererToPng.PageScale);
            sheetRendererToPng.ToImage(0, _destFilesPath + "NET47544.png");

            SheetRender sheetRendererToJpg = new SheetRender(worksheet, GetSaveOptionsForJpg());
            sheetRendererToJpg.ToImage(0, _destFilesPath + "NET47544.jpg");
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


