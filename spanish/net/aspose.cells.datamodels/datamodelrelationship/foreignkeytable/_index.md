---
title: "DataModelRelationship.ForeignKeyTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataModelRelationship. Obtiene el nombre de la tabla de clave externa para esta relación"
type: docs
url: /es/net/aspose.cells.datamodels/datamodelrelationship/foreignkeytable/
---
## DataModelRelationship.ForeignKeyTable property

Obtiene el nombre de la tabla de clave foránea para esta relación.

```csharp
public string ForeignKeyTable { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipPropertyForeignKeyTableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para crear un contexto significativo
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");

            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");

            try
            {
                // Acceder a la primera relación si existe
                DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];

                if (relationship != null)
                {
                    // Mostrar el valor de la propiedad ForeignKeyTable (solo lectura)
                    Console.WriteLine("Foreign Key Table: " + relationship.ForeignKeyTable);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // Guarda el libro de trabajo
                workbook.Save("ForeignKeyTableDemo.xlsx");
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

* class [DataModelRelationship](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


