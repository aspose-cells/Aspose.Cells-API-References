---
title: "Clase DataModelTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.DataModels.DataModelTable. Representa las propiedades de una única tabla en el modelo de datos de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.datamodels/datamodeltable/
---
## DataModelTable class

Representa las propiedades de una única tabla en el modelo de datos de la hoja de cálculo.

```csharp
public class DataModelTable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ConnectionName](../../aspose.cells.datamodels/datamodeltable/connectionname/) { get; } | Obtiene el nombre de conexión de la tabla del modelo de datos. |
| [Id](../../aspose.cells.datamodels/datamodeltable/id/) { get; } | Obtiene el id de la tabla del modelo de datos. |
| [Name](../../aspose.cells.datamodels/datamodeltable/name/) { get; } | Obtiene el nombre de la tabla del modelo de datos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using Aspose.Cells.Pivot;
    using System;

    public class DataModelsClassDataModelTableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para crear una tabla
            worksheet.Cells["A1"].PutValue("ProductID");
            worksheet.Cells["B1"].PutValue("ProductName");
            worksheet.Cells["A2"].PutValue(101);
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["A3"].PutValue(102);
            worksheet.Cells["B3"].PutValue("Monitor");

            // Crear un ListObject (tabla)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "ProductsTable";

            // Acceder al DataModelTable
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Mostrar propiedades del DataModelTable
            Console.WriteLine("Data Model Table Properties:");
            Console.WriteLine($"ID: {dataModelTable.Id}");
            Console.WriteLine($"Name: {dataModelTable.Name}");
            Console.WriteLine($"Connection Name: {dataModelTable.ConnectionName}");

            // Crear una tabla dinámica usando el DataModelTable
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "ProductName");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "ProductID");

            // Guarda el libro de trabajo
            workbook.Save("DataModelTableDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


