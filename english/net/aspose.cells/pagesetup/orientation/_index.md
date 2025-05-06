---
title: PageSetup.Orientation
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents page print orientation
type: docs
url: /net/aspose.cells/pagesetup/orientation/
---
## PageSetup.Orientation property

Represents page print orientation.

```csharp
public PageOrientationType Orientation { get; set; }
```

### Examples

```csharp
// Called: worksheet.PageSetup.Orientation = Aspose.Cells.PageOrientationType.Portrait;
[Test]
        public void Property_Orientation()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET46447/&quot;;

            string FileName = &quot;HCP_Fees_for_Services_and_Consultancy_20181114114513242.html&quot;;
            string inputfileName = filePath + FileName;
            string outputfileName = CreateFolder(filePath) + &quot;checkdatasa.xls&quot;;

            Aspose.Cells.HtmlLoadOptions hTMLLoad = new Aspose.Cells.HtmlLoadOptions(LoadFormat.Html);
            hTMLLoad.IgnoreNotPrinted = true;
            hTMLLoad.AutoFitColsAndRows = true;

            Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(inputfileName, hTMLLoad);
            Aspose.Cells.Worksheet worksheet = null;

            if (workbook != null)
            {
                worksheet = workbook.Worksheets[0];
                worksheet.PageSetup.PrintTitleRows = &quot;$1:$3&quot;;
            }
            //workbook.Save(outputfileName,SaveFormat.Xlsx); 
            worksheet.PageSetup.Orientation = Aspose.Cells.PageOrientationType.Portrait;

            Assert.AreEqual(worksheet.Cells[&quot;B3&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 244, 200, 66));
            Assert.AreEqual(worksheet.Cells[&quot;B4&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 218, 238, 243));
            Assert.AreEqual(worksheet.Cells[&quot;B5&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 142, 93, 39));
            worksheet.Workbook.Save(outputfileName);
        }
```

### See Also

* enum [PageOrientationType](../../pageorientationtype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


