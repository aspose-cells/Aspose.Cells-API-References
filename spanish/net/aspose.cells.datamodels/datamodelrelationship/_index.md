---
title: "Clase DataModelRelationship"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.DataModels.DataModelRelationship clase. Representa una única relación en el modelo de datos de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.datamodels/datamodelrelationship/
---
## DataModelRelationship class

Representa una única relación en el modelo de datos de la hoja de cálculo.

```csharp
public class DataModelRelationship
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ForeignKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/foreignkeycolumn/) { get; } | Obtiene el nombre de la columna de tabla de clave foránea para esta relación. |
| [ForeignKeyTable](../../aspose.cells.datamodels/datamodelrelationship/foreignkeytable/) { get; } | Obtiene el nombre de la tabla de clave foránea para esta relación. |
| [PrimaryKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/primarykeycolumn/) { get; } | Obtiene el nombre de la columna de tabla de clave primaria para esta relación. |
| [PrimaryKeyTable](../../aspose.cells.datamodels/datamodelrelationship/primarykeytable/) { get; } | Obtiene el nombre de la tabla de clave primaria para esta relación. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelsClassDataModelRelationshipDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra para la demostración
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");
            worksheet.Cells["A4"].PutValue("OrderDate");
            
            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");
            worksheet.Cells["C4"].PutValue("ContactName");

            // Esto demuestra el acceso a las propiedades de una relación existente
            // En un escenario real, obtendrías esto del DataModel
            DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];
            if (relationship != null)
            {
                // Mostrar propiedades de relación (solo lectura)
                Console.WriteLine("Sample Data Model Relationship Properties:");
                Console.WriteLine("Primary Key Table: " + relationship.PrimaryKeyTable);
                Console.WriteLine("Primary Key Column: " + relationship.PrimaryKeyColumn);
                Console.WriteLine("Foreign Key Table: " + relationship.ForeignKeyTable);
                Console.WriteLine("Foreign Key Column: " + relationship.ForeignKeyColumn);
            }
            else
            {
                Console.WriteLine("No data model relationships found");
            }

            // Guarda el libro de trabajo
            workbook.Save("DataModelRelationshipDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


