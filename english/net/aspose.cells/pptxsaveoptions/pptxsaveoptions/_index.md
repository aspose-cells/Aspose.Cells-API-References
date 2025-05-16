---
title: PptxSaveOptions.PptxSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: PptxSaveOptions constructor. Represents the pptx save options
type: docs
url: /net/aspose.cells/pptxsaveoptions/pptxsaveoptions/
---
## PptxSaveOptions() {#constructor}

Represents the pptx save options.

```csharp
public PptxSaveOptions()
```

### Examples

```csharp
// Called: PptxSaveOptions saveOptions = new PptxSaveOptions();
public void PptxSaveOptions_Constructor()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    PptxSaveOptions saveOptions = new PptxSaveOptions();
    saveOptions.IgnoreHiddenRows = true;
    wb.Save(Constants.destPath + "example.pptx", saveOptions);
    string slide1 = GetEntryText(Constants.destPath + "example.pptx", @"ppt\slides\slide1.xml");
    Assert.IsTrue(slide1.IndexOf("Qtr1") == -1);
}
```

### See Also

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PptxSaveOptions(bool) {#constructor_1}

Represents options of saving .pptx file.

```csharp
public PptxSaveOptions(bool saveAsImage)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveAsImage | Boolean | If True, the workbook will be converted into some pictures of .pptx file. If False, the workbook will be converted into some tables of .pptx file. |

### Examples

```csharp
namespace AsposeCellsExamples.PptxSaveOptionsMethodCtorWithBooleanDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Slides;
    using System;

    public class PptxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            try
            {
                // Call the #ctor method with boolean parameter
                bool saveAsImage = true;
                PptxSaveOptions options = new PptxSaveOptions(saveAsImage);

                // Set additional properties
                options.IgnoreHiddenRows = true;
                options.ExportViewType = SlideViewType.View;

                // Save the workbook with PPTX options
                workbook.Save("PptxSaveOptionsCtorDemo.pptx", options);

                Console.WriteLine("PptxSaveOptions constructor executed successfully with parameter: " + saveAsImage);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PptxSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


