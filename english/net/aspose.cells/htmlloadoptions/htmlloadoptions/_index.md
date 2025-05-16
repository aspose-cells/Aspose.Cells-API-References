---
title: HtmlLoadOptions.HtmlLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: HtmlLoadOptions constructor. Creates an options of loading the file
type: docs
url: /net/aspose.cells/htmlloadoptions/htmlloadoptions/
---
## HtmlLoadOptions() {#constructor}

Creates an options of loading the file.

```csharp
public HtmlLoadOptions()
```

### Examples

```csharp
// Called: HtmlLoadOptions loadOptions = new HtmlLoadOptions();
public void HtmlLoadOptions_Constructor()
{
    HtmlLoadOptions loadOptions = new HtmlLoadOptions();
    loadOptions.SupportDivTag = true;
    Workbook wb = new Workbook(Constants.HtmlPath + "example.html", loadOptions);
    Assert.AreEqual("Internal", wb.Worksheets[0].Cells["B1"].StringValue);
    Assert.AreEqual("Internal", wb.Worksheets[0].Cells["B1"].StringValue);
    Assert.AreEqual("testingggg", wb.Worksheets[0].Cells["B3"].StringValue);
    Assert.AreEqual("testinggggerertwrt", wb.Worksheets[0].Cells["B4"].StringValue);
}
```

### See Also

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlLoadOptions(LoadFormat) {#constructor_1}

Creates an options of loading the file.

```csharp
public HtmlLoadOptions(LoadFormat loadFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loading format. |

### Examples

```csharp
namespace AsposeCellsExamples.HtmlLoadOptionsMethodCtorWithLoadFormatDemo
{
    using Aspose.Cells;
    using System;

    public class HtmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Create HtmlLoadOptions instance using constructor with LoadFormat parameter
                HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);

                // Set some properties of the HtmlLoadOptions
                loadOptions.AutoFitColsAndRows = true;
                loadOptions.SupportDivTag = true;
                loadOptions.DeleteRedundantSpaces = true;

                // Create a workbook using the load options
                Workbook workbook = new Workbook("input.html", loadOptions);

                // Access the first worksheet
                Worksheet worksheet = workbook.Worksheets[0];

                // Display some information about the loaded HTML
                Console.WriteLine("HTML loaded successfully with LoadFormat.Html");
                Console.WriteLine($"Worksheet name: {worksheet.Name}");
                Console.WriteLine($"Cells count: {worksheet.Cells.MaxDataRow + 1} rows x {worksheet.Cells.MaxDataColumn + 1} columns");

                // Save the workbook
                workbook.Save("HtmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading HTML file: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [LoadFormat](../../loadformat/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


