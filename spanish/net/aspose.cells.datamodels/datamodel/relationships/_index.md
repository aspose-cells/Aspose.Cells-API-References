---
title: "DataModel.Relationships"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataModel. Obtiene todas las relaciones de las tablas en el modelo de datos"
type: docs
url: /es/net/aspose.cells.datamodels/datamodel/relationships/
---
## DataModel.Relationships property

Obtiene todas las relaciones de las tablas en el modelo de datos.

```csharp
public DataModelRelationshipCollection Relationships { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelPropertyRelationshipsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Acceder al DataModel desde el libro de trabajo
                DataModel dataModel = workbook.DataModel;

                // Mostrar el valor actual de la propiedad Relationships (solo lectura)
                Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

                // Iterar a través de las relaciones si existen
                foreach (DataModelRelationship relationship in dataModel.Relationships)
                {
                    Console.WriteLine("Relationship found: " + relationship);
                }

                // Guarda el libro de trabajo
                workbook.Save("RelationshipsDemo.xlsx");
                Console.WriteLine("Relationships demonstration completed successfully.");
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

* class [DataModelRelationshipCollection](../../datamodelrelationshipcollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


