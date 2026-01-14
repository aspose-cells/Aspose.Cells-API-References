---
title: DocxSaveOptions.SaveAsEditableShapes
second_title: Aspose.Cells for .NET API Reference
description: DocxSaveOptions property. Save all drawing objects as editable shapes in the word file so you can edit them in Word
type: docs
url: /net/aspose.cells/docxsaveoptions/saveaseditableshapes/
---
## DocxSaveOptions.SaveAsEditableShapes property

Save all drawing objects as editable shapes in the word file, so you can edit them in Word.

```csharp
public bool SaveAsEditableShapes { get; set; }
```

### Remarks

Only for charts.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertySaveAsEditableShapesDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet and add sample data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Editable Shapes Demo";

            try
            {
                // Initialize DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Display the default value of SaveAsEditableShapes property
                Console.WriteLine("Default SaveAsEditableShapes value: " + saveOptions.SaveAsEditableShapes);

                // Set SaveAsEditableShapes to true to demonstrate its usage
                saveOptions.SaveAsEditableShapes = true;
                Console.WriteLine("SaveAsEditableShapes set to: " + saveOptions.SaveAsEditableShapes);

                // Save the workbook as DOCX with the configured options
                workbook.Save("SaveAsEditableShapesDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with SaveAsEditableShapes option.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


