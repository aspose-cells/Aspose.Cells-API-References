---
title: LoadOptions.CultureInfo
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets or sets the system culture info at the time the file was loaded
type: docs
url: /net/aspose.cells/loadoptions/cultureinfo/
---
## LoadOptions.CultureInfo property

Gets or sets the system culture info at the time the file was loaded.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Examples

```csharp
// Called: options.CultureInfo = culture;
[Test]
        public void Property_CultureInfo()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA41994/";
            LoadOptions options = new LoadOptions();
            CultureInfo culture = new CultureInfo("en-US");
            options.CultureInfo = culture;
            Workbook wb = new Workbook(filePath + "人员总结计划2.xlsx", options);
            Assert.AreEqual(414, wb.Worksheets[0].Cells.GetColumnWidthPixel(6));

            wb.Save(CreateFolder(filePath) + "out.html");
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


