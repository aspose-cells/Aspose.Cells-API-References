---
title: "WorkbookMetadata.CustomDocumentProperties"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookMetadata. Devuelve una colección DocumentProperty que representa todas las propiedades de documento personalizadas de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.metadata/workbookmetadata/customdocumentproperties/
---
## WorkbookMetadata.CustomDocumentProperties property

Devuelve una colección [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) que representa todas las propiedades de documento personalizadas de la hoja de cálculo.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Rutas de origen y destino
            string sourcePath = "example.xlsx";
            string destPath = "output.xlsx";

            // Crear opciones de metadatos para propiedades de documento
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // Inicializar metadatos del libro de trabajo
            WorkbookMetadata meta = new WorkbookMetadata(sourcePath, options);
            
            // Agregar propiedad de documento personalizada
            meta.CustomDocumentProperties.Add("Author", "John Doe");
            
            // Guardar el libro de trabajo con metadatos
            meta.Save(destPath);
            
            // Verificar la propiedad personalizada
            Workbook workbook = new Workbook(destPath);
            Console.WriteLine("Custom Property Value: " + 
                workbook.CustomDocumentProperties["Author"].Value);
        }
    }
}
```

### Ver también

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


