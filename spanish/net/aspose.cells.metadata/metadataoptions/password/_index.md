---
title: "MetadataOptions.Password"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "MetadataOptions property. Representa la contraseña de cifrado del archivo Workbook"
type: docs
url: /es/net/aspose.cells.metadata/metadataoptions/password/
---
## MetadataOptions.Password property

Representa la contraseña de cifrado del archivo Workbook.

```csharp
public string Password { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class MetadataOptionsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Crear opciones de metadatos con protección por contraseña
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "secure_password123";
            
            // Crear un nuevo libro de trabajo y guardarlo primero
            Workbook workbook = new Workbook();
            string filePath = "ProtectedMetadata.xlsx";
            workbook.Save(filePath);
            
            // Cargar metadatos del archivo guardado
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);
            
            // Agregar propiedad de documento personalizada
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // Guardar con metadatos
            metadata.Save(filePath);
        }
    }
}
```

### Ver también

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


