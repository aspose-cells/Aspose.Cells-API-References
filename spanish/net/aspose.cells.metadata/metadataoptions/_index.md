---
title: "Clase MetadataOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Metadata.MetadataOptions. Representa las opciones de carga de metadatos del archivo"
type: docs
url: /es/net/aspose.cells.metadata/metadataoptions/
---
## MetadataOptions class

Representa las opciones de carga de metadatos del archivo.

```csharp
public class MetadataOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [MetadataOptions](metadataoptions/)(MetadataType) | Crea una opción para cargar los metadatos. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [KeyLength](../../aspose.cells.metadata/metadataoptions/keylength/) { get; set; } | La longitud de la clave. |
| [MetadataType](../../aspose.cells.metadata/metadataoptions/metadatatype/) { get; } | Obtiene y establece el tipo de los metadatos que se están cargando. |
| [Password](../../aspose.cells.metadata/metadataoptions/password/) { get; set; } | Representa la contraseña de cifrado del archivo Workbook. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class MetadataOptionsDemo
    {
        public static void MetadataOptionsExample()
        {
            // Crea una instancia de MetadataOptions con un MetadataType específico
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Establecer propiedades
            options.Password = "your_password";
            options.KeyLength = 256;

            // Carga los metadatos de un libro de trabajo existente
            WorkbookMetadata metadata = new WorkbookMetadata("MetadataOptionsExample_original.xlsx", options);

            // Agrega una propiedad de documento personalizada
            metadata.CustomDocumentProperties.Add("Author", "John Doe");

            // Guarda los cambios de los metadatos en un archivo nuevo
            metadata.Save("MetadataOptionsExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


