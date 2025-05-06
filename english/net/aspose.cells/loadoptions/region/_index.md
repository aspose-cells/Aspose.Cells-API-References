---
title: LoadOptions.Region
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets or sets the system regional settings based on CountryCode at the time the file was loaded
type: docs
url: /net/aspose.cells/loadoptions/region/
---
## LoadOptions.Region property

Gets or sets the system regional settings based on CountryCode at the time the file was loaded.

```csharp
public CountryCode Region { get; set; }
```

### Remarks

If you do not want to use the region saved in the file, please reset it after reading the file.

### Examples

```csharp
// Called: options.Region = CountryCode.USA;
[Test]
        public void Property_Region()
        {
            LoadOptions options = new LoadOptions();
            options.Region = CountryCode.USA;
            Workbook wb = new Workbook(Constants.sourcePath + &quot;JAVA41337.xlsx&quot;, options);

            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
           
            wb.Worksheets.ActiveSheetName = &quot;filenet&quot;;
            wb.Save(_destFilesPath + &quot;JAVA41337.html&quot;, saveOptions);
            //using(MemoryStream ms = new MemoryStream())
            //{
            //    wb.Save(ms, saveOptions);
            //    Assert.IsTrue(ms.Length &lt; 154000);
            //}

           
        }
```

### See Also

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


