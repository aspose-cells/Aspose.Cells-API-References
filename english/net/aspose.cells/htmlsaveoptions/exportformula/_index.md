---
title: HtmlSaveOptions.ExportFormula
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportformula/
---
## HtmlSaveOptions.ExportFormula property

Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value.

```csharp
public bool ExportFormula { get; set; }
```

### Examples

```csharp
// Called: saveOptions.ExportFormula = false;
[Test]
        public void Property_ExportFormula()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "JAVA41327And41340.xlsx");
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = (true);
            saveOptions.ExportFormula = false;
            wb.Worksheets.ActiveSheetIndex = wb.Worksheets["liste élèves"].Index;
            wb.Save(_destFilesPath + "JAVA41327And41340.html", saveOptions);

            //using (MemoryStream ms = new MemoryStream())
            {
            //    wb.Save(ms, saveOptions);
            //    string text = Encoding.UTF8.GetString(ms.GetBuffer(), 0, (int)ms.Length);
            string text = File.ReadAllText(_destFilesPath + "JAVA41327And41340.html");

                Assert.IsTrue(text.IndexOf("<td class='x192' align='right'>0</td>") != -1);
                //<td class='x187' align='right' style='text-align:right;'>0</td>
                Assert.IsTrue(text.IndexOf("<font class=\"font4\" style=\"text-decoration: none;\">sur l'onglet</font>") != -1);
            }
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


