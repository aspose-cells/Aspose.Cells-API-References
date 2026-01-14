---
title: EbookLoadOptions.EbookLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: EbookLoadOptions constructor. Creates an option for loading the ebook file
type: docs
url: /net/aspose.cells/ebookloadoptions/ebookloadoptions/
---
## EbookLoadOptions() {#constructor}

Creates an option for loading the ebook file.

```csharp
public EbookLoadOptions()
```

### Examples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class EbookLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Create an instance of EbookLoadOptions using the constructor
            EbookLoadOptions options = new EbookLoadOptions();

            // Set some basic properties
            options.Password = "secure123";
            options.Encoding = Encoding.UTF8;
            options.LoadFormulas = true;
            
            // Load an ebook file with the specified options
            Workbook workbook = new Workbook("sample.epub", options);
            
            // Save as Excel file
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EbookLoadOptions(LoadFormat) {#constructor_1}

Creates an option of loading the ebook file.

```csharp
public EbookLoadOptions(LoadFormat loadFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loading format |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EbookLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Create EbookLoadOptions instance with LoadFormat parameter
                EbookLoadOptions options = new EbookLoadOptions(LoadFormat.Epub);

                // Display confirmation
                Console.WriteLine("EbookLoadOptions created successfully with LoadFormat.Epub");

                // Example usage: Load a workbook with these options
                Workbook workbook = new Workbook("sample.epub", options);
                Console.WriteLine("Workbook loaded successfully with EbookLoadOptions");

                // Save the result
                workbook.Save("EbookLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [LoadFormat](../../loadformat/)
* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


