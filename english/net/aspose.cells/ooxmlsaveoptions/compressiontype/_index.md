---
title: OoxmlSaveOptions.CompressionType
second_title: Aspose.Cells for .NET API Reference
description: OoxmlSaveOptions property. Gets and sets the compression type for ooxml file
type: docs
url: /net/aspose.cells/ooxmlsaveoptions/compressiontype/
---
## OoxmlSaveOptions.CompressionType property

Gets and sets the compression type for ooxml file.

```csharp
public OoxmlCompressionType CompressionType { get; set; }
```

### Remarks

The default value is OoxmlCompressionType.Level2.

### Examples

```csharp
// Called: saveOptions.CompressionType = OoxmlCompressionType.Level6; // A good balance of speed and compression efficiency
public static void OoxmlSaveOptions_Property_CompressionType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // Create OoxmlSaveOptions and set the compression type
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6; // A good balance of speed and compression efficiency

            // Save the workbook with the specified compression type
            workbook.Save("OoxmlCompressionTypeExample.xlsx", saveOptions);

            Console.WriteLine("Workbook saved with OoxmlCompressionType.Level6 compression.");
        }
```

### See Also

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


