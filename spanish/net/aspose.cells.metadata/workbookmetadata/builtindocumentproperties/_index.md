---
title: "WorkbookMetadata.BuiltInDocumentProperties"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookMetadata. Devuelve una colección DocumentProperty que representa todas las propiedades de documento incorporadas de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.metadata/workbookmetadata/builtindocumentproperties/
---
## WorkbookMetadata.BuiltInDocumentProperties property

Devuelve una colección [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) que representa todas las propiedades de documento integradas de la hoja de cálculo.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class WorkbookMetadataPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Guardar el libro de trabajo en un archivo
                string filePath = "BuiltInDocumentPropertiesDemo.xlsx";
                workbook.Save(filePath);

                // Crear opciones de metadatos para propiedades de documento
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // Inicializar metadatos del libro de trabajo
                WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

                // Acceder a las propiedades de documento incorporadas (solo lectura)
                var builtInProps = metadata.BuiltInDocumentProperties;

                // Mostrar algunas propiedades de documento incorporadas
                Console.WriteLine("Built-in Document Properties:");
                Console.WriteLine("Author: " + builtInProps.Author);
                Console.WriteLine("Title: " + builtInProps.Title);
                Console.WriteLine("Subject: " + builtInProps.Subject);
                Console.WriteLine("Created Time: " + builtInProps.CreatedTime);
                Console.WriteLine("Last Saved By: " + builtInProps.LastSavedBy);
                Console.WriteLine("Total Editing Time: " + builtInProps.TotalEditingTime);

                // Modificar algunas propiedades incorporadas (ya que son de lectura-escritura)
                builtInProps.Author = "Aspose Developer";
                builtInProps.Title = "BuiltIn Properties Demo";
                builtInProps.Subject = "Demonstrating BuiltInDocumentProperties";
                builtInProps.Company = "Aspose";
                builtInProps.Comments = "This demonstrates the BuiltInDocumentProperties API";

                // Guardar los cambios de los metadatos
                metadata.Save(filePath);

                Console.WriteLine("\nBuilt-in properties have been updated and saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


