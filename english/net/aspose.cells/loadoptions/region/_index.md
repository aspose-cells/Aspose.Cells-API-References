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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyRegionDemo
    {
        public static void Run()
        {
            // Create load options for HTML file
            LoadOptions loadOpts = new LoadOptions(LoadFormat.Html);
            
            // Set the region to USA
            loadOpts.Region = CountryCode.USA;
            
            // Load the HTML file with the specified region settings
            Workbook wb = new Workbook("example.html", loadOpts);
            
            // Access the first worksheet
            Worksheet ws = wb.Worksheets[0];
            
            // Demonstrate region-specific formatting by checking a cell's style
            Style style = ws.Cells["A1"].GetStyle();
            Console.WriteLine("Font used in cell A1: " + style.Font.Name);
            Console.WriteLine("Region used for loading: " + loadOpts.Region);
        }
    }
}
```

### See Also

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


