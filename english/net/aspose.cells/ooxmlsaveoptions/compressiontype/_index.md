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
// Called: options.CompressionType = OoxmlCompressionType.Level6;
[Test]
        public void Property_CompressionType()
        {
            Workbook workbook = new Workbook();
            OoxmlSaveOptions options = new OoxmlSaveOptions();
            options.CompressionType = OoxmlCompressionType.Level6;
            workbook.Save(Constants.destPath + "CellsNet46907.xlsx", options);
        }
```

### See Also

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


