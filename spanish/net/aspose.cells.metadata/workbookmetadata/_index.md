---
title: "Clase WorkbookMetadata"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Metadata.WorkbookMetadata. Representa los metadatos"
type: docs
url: /es/net/aspose.cells.metadata/workbookmetadata/
---
## WorkbookMetadata class

Representa los metadatos.

```csharp
public class WorkbookMetadata
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [WorkbookMetadata](workbookmetadata/#constructor)(Stream, MetadataOptions) | Crea el objeto de metadatos. |
| [WorkbookMetadata](workbookmetadata/#constructor_1)(string, MetadataOptions) | Crea el objeto de metadatos. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BuiltInDocumentProperties](../../aspose.cells.metadata/workbookmetadata/builtindocumentproperties/) { get; } | Devuelve una colección de [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) que representa todas las propiedades de documento incorporadas de la hoja de cálculo. |
| [CustomDocumentProperties](../../aspose.cells.metadata/workbookmetadata/customdocumentproperties/) { get; } | Devuelve una colección de [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) que representa todas las propiedades de documento personalizadas de la hoja de cálculo. |
| [Options](../../aspose.cells.metadata/workbookmetadata/options/) { get; } | Obtiene las opciones de los metadatos. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save)(Stream) | Guarda los metadatos modificados en el flujo. |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save_1)(string) | Guarda los metadatos modificados en el archivo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using Aspose.Cells.Properties;
    using System;
    using System.IO;

    public class WorkbookMetadataDemo
    {
        public static void WorkbookMetadataExample()
        {
            // Crea una instancia de MetadataOptions
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Crea una instancia de WorkbookMetadata con un nombre de archivo y opciones
            WorkbookMetadata meta = new WorkbookMetadata("WorkbookMetadataExample_original.xlsx", options);

            // Agrega una propiedad de documento personalizada
            meta.CustomDocumentProperties.Add("test", "test");

            // Guarda los metadatos en un archivo nuevo
            meta.Save("WorkbookMetadataExample.xlsx");

            // Demuestra el acceso a propiedades de documento incorporadas
            BuiltInDocumentPropertyCollection builtInProps = meta.BuiltInDocumentProperties;
            Console.WriteLine("Author: " + builtInProps.Author);
            Console.WriteLine("Title: " + builtInProps.Title);

            // Demuestra el acceso a propiedades de documento personalizadas
            CustomDocumentPropertyCollection customProps = meta.CustomDocumentProperties;
            foreach (DocumentProperty prop in customProps)
            {
                Console.WriteLine("Custom Property - Name: " + prop.Name + ", Value: " + prop.Value);
            }

            // Guarda los metadatos en un flujo
            using (FileStream stream = new FileStream("WorkbookMetadataExample2.xlsx", FileMode.Create, FileAccess.Write))
            {
                meta.Save(stream);
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


