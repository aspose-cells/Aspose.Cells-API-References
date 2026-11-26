---
title: "Enumeración MetadataType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Metadata.MetadataType. Representa el tipo de metadatos"
type: docs
url: /es/net/aspose.cells.metadata/metadatatype/
---
## MetadataType enumeration

Representa el tipo de metadatos.

```csharp
[Flags]
public enum MetadataType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Encryption | `1` | Encripta el archivo. |
| Decryption | `2` | Desencripta el archivo. |
| DocumentProperties | `4` | Cargar las propiedades del archivo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Metadata;
    using Aspose.Cells.Properties;
    using System;
    using System.IO;

    public class MetadataTypeDemo
    {
        public static void MetadataTypeExample()
        {
            // Definir la ruta del archivo
            string filePath = "MetadataTypeExample_original.xlsx";

            // Crear MetadataOptions para DocumentProperties
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Cargar los metadatos del libro de trabajo
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

            // Acceder a las propiedades de documento incorporadas
            BuiltInDocumentPropertyCollection builtInProperties = metadata.BuiltInDocumentProperties;

            // Acceder a las propiedades de documento personalizadas
            CustomDocumentPropertyCollection customProperties = metadata.CustomDocumentProperties;

            // Mostrar algunas propiedades incorporadas
            Console.WriteLine("Title: " + builtInProperties["Title"]);
            Console.WriteLine("Author: " + builtInProperties["Author"]);
            Console.WriteLine("Company: " + builtInProperties["Company"]);

            // Agregar una propiedad personalizada
            customProperties.Add("MyCustomProperty", "CustomValue");

            // guardar en un archivo diferente
            string newFilePath = "MetadataTypeExample.xlsx";
            metadata.Save(newFilePath);

            Console.WriteLine("Metadata updated and saved successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


