---
title: HtmlLoadOptions.AutoFitColsAndRows
second_title: Aspose.Cells for .NET API Reference
description: HtmlLoadOptions property. Indicates whether autofit columns and rows. The default value is false
type: docs
url: /net/aspose.cells/htmlloadoptions/autofitcolsandrows/
---
## HtmlLoadOptions.AutoFitColsAndRows property

Indicates whether auto-fit columns and rows. The default value is false.

```csharp
public bool AutoFitColsAndRows { get; set; }
```

### Examples

```csharp
// Called: options.AutoFitColsAndRows = true;
[Test]
        public void Property_AutoFitColsAndRows()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET44595And44596And44597/";

            string savePath = CreateFolder(filePath);
            HtmlLoadOptions options = new HtmlLoadOptions();
            options.SupportDivTag = true;
            options.AutoFitColsAndRows = true;
            Workbook wb = null;
            wb = new Workbook(filePath + "test2.html", options);
            wb.Save(savePath + "44595_out.xlsx");

            wb = new Workbook(filePath + "test3.html", options);
            wb.Save(savePath + "44596_out.xlsx");

            wb = new Workbook(filePath + "test4.html");
            wb.Save(savePath + "44597_out.xlsx");
        }
```

### See Also

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


