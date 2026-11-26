---
title: "DataModelRelationship.PrimaryKeyTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataModelRelationship. Obtiene el nombre de la tabla de clave primaria para esta relación"
type: docs
url: /es/net/aspose.cells.datamodels/datamodelrelationship/primarykeytable/
---
## DataModelRelationship.PrimaryKeyTable property

Obtiene el nombre de la tabla de clave primaria para esta relación.

```csharp
public string PrimaryKeyTable { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipPropertyPrimaryKeyTableDemo
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
                    // Mostrar el valor de la propiedad PrimaryKeyTable (solo lectura)
                    Console.WriteLine("Primary Key Table: " + relationship.PrimaryKeyTable);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // Guarda el libro de trabajo
                workbook.Save("PrimaryKeyTableDemo.xlsx");
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


