---
title: XlsbSaveOptions.XlsbSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: XlsbSaveOptions constructor. Creates xlsb file save options
type: docs
url: /net/aspose.cells/xlsbsaveoptions/xlsbsaveoptions/
---
## XlsbSaveOptions() {#constructor}

Creates xlsb file save options.

```csharp
public XlsbSaveOptions()
```

### Examples

```csharp
// Called: XlsbSaveOptions saveOptions = new XlsbSaveOptions();
public void XlsbSaveOptions_Constructor()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells["A1"].PutValue("A1");
    cells["B1"].PutValue("B1");
    cells["C1"].PutValue("C1");
    XlsbSaveOptions saveOptions = new XlsbSaveOptions();
    saveOptions.ExportAllColumnIndexes = true;
    workbook.Save(Constants.destPath + "example.xlsb", saveOptions);
    saveOptions.ExportAllColumnIndexes = false;
    workbook.Save(Constants.destPath + "example.xlsb", saveOptions);
}
```

### See Also

* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XlsbSaveOptions(SaveFormat) {#constructor_1}

Creates xlsb file save options.

```csharp
[Obsolete("Use XlsbSaveOptions() constructor instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public XlsbSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The save format . It must be xlsb. |

### Remarks

NOTE: This constructor is now obsolete. Instead, please use XlsbSaveOptions() constructor. This property will be removed 12 months later since January 2021. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples.XlsbSaveOptionsMethodCtorWithSaveFormatDemo
{
    using Aspose.Cells;
    using System;

    public class XlsbSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data to worksheet
            worksheet.Cells["A1"].PutValue("Sample XLSB Save Options Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            try
            {
                // Call the #ctor method with SaveFormat parameter
                XlsbSaveOptions saveOptions = new XlsbSaveOptions(SaveFormat.Xlsb);
                
                // Set additional properties
                saveOptions.CompressionType = OoxmlCompressionType.Level6;
                saveOptions.ExportAllColumnIndexes = true;
                
                Console.WriteLine("XlsbSaveOptions constructor executed successfully with SaveFormat.Xlsb");
                
                // Save the workbook with the specified options
                workbook.Save("XlsbSaveOptionsDemo.xlsb", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XlsbSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [SaveFormat](../../saveformat/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


