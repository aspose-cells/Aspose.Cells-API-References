---
title: "DataModelRelationship.PrimaryKeyColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataModelRelationship. Obtiene el nombre de la columna de tabla de clave primaria para esta relación"
type: docs
url: /es/net/aspose.cells.datamodels/datamodelrelationship/primarykeycolumn/
---
## DataModelRelationship.PrimaryKeyColumn property

Obtiene el nombre de la columna de tabla de clave primaria para esta relación.

```csharp
public string PrimaryKeyColumn { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipPropertyPrimaryKeyColumnDemo
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
                    // Mostrar el valor de la propiedad PrimaryKeyColumn (solo lectura)
                    Console.WriteLine("Primary Key Column: " + relationship.PrimaryKeyColumn);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // Guarda el libro de trabajo
                workbook.Save("PrimaryKeyColumnDemo.xlsx");
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


