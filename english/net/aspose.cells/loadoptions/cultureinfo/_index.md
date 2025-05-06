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
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA41994/&quot;;
            LoadOptions options = new LoadOptions();
            CultureInfo culture = new CultureInfo(&quot;en-US&quot;);
            options.CultureInfo = culture;
            Workbook wb = new Workbook(filePath + &quot;人员总结计划2.xlsx&quot;, options);
            Assert.AreEqual(414, wb.Worksheets[0].Cells.GetColumnWidthPixel(6));

            wb.Save(CreateFolder(filePath) + &quot;out.html&quot;);
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


