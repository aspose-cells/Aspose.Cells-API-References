---
title: "DataModelRelationship.ForeignKeyColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataModelRelationship. Obtiene el nombre de la columna de tabla de clave externa para esta relación"
type: docs
url: /es/net/aspose.cells.datamodels/datamodelrelationship/foreignkeycolumn/
---
## DataModelRelationship.ForeignKeyColumn property

Obtiene el nombre de la columna de tabla de clave foránea para esta relación.

```csharp
public string ForeignKeyColumn { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipPropertyForeignKeyColumnDemo
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
                    // Mostrar el valor de la propiedad ForeignKeyColumn (solo lectura)
                    Console.WriteLine("Foreign Key Column: " + relationship.ForeignKeyColumn);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // Guarda el libro de trabajo
                workbook.Save("ForeignKeyColumnDemo.xlsx");
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


