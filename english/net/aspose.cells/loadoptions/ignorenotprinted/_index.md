---
title: LoadOptions.IgnoreNotPrinted
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Ignore the data which are not printed if directly printing the file
type: docs
url: /net/aspose.cells/loadoptions/ignorenotprinted/
---
## LoadOptions.IgnoreNotPrinted property

Ignore the data which are not printed if directly printing the file

```csharp
public bool IgnoreNotPrinted { get; set; }
```

### Remarks

Only for xlsx file.

### Examples

```csharp
// Called: hTMLLoad.IgnoreNotPrinted = true;
[Test]
        public void Property_IgnoreNotPrinted()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET46447/";

            string FileName = "HCP_Fees_for_Services_and_Consultancy_20181114114513242.html";
            string inputfileName = filePath + FileName;
            string outputfileName = CreateFolder(filePath) + "checkdatasa.xls";

            Aspose.Cells.HtmlLoadOptions hTMLLoad = new Aspose.Cells.HtmlLoadOptions(LoadFormat.Html);
            hTMLLoad.IgnoreNotPrinted = true;
            hTMLLoad.AutoFitColsAndRows = true;

            Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(inputfileName, hTMLLoad);
            Aspose.Cells.Worksheet worksheet = null;

            if (workbook != null)
            {
                worksheet = workbook.Worksheets[0];
                worksheet.PageSetup.PrintTitleRows = "$1:$3";
            }
            //workbook.Save(outputfileName,SaveFormat.Xlsx); 
            worksheet.PageSetup.Orientation = Aspose.Cells.PageOrientationType.Portrait;

            Assert.AreEqual(worksheet.Cells["B3"].GetStyle().ForegroundColor, Color.FromArgb(255, 244, 200, 66));
            Assert.AreEqual(worksheet.Cells["B4"].GetStyle().ForegroundColor, Color.FromArgb(255, 218, 238, 243));
            Assert.AreEqual(worksheet.Cells["B5"].GetStyle().ForegroundColor, Color.FromArgb(255, 142, 93, 39));
            worksheet.Workbook.Save(outputfileName);
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


