---
title: "MetadataOptions.KeyLength"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "MetadataOptions property. La longitud de la clave"
type: docs
url: /es/net/aspose.cells.metadata/metadataoptions/keylength/
---
## MetadataOptions.KeyLength property

La longitud de la clave.

```csharp
public int KeyLength { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class MetadataOptionsPropertyKeyLengthDemo
    {
        public static void Run()
        {
            // Crear opciones de metadatos con tipo de propiedades de documento
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // Establecer propiedades de cifrado incluyendo KeyLength
            options.Password = "secure_password";
            options.KeyLength = 256; // Using 256-bit encryption
            
            // Crear metadatos para un nuevo libro de trabajo
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);
            
            // Agregar propiedad personalizada
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // Guardar con cifrado
            metadata.Save("encrypted_sample.xlsx");
        }
    }
}
```

### Ver también

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


