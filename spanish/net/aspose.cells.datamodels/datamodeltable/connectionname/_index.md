---
title: "DataModelTable.ConnectionName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataModelTable. Obtiene el nombre de conexión de la tabla de modelo de datos"
type: docs
url: /es/net/aspose.cells.datamodels/datamodeltable/connectionname/
---
## DataModelTable.ConnectionName property

Obtiene el nombre de conexión de la tabla del modelo de datos.

```csharp
public string ConnectionName { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using Aspose.Cells.Pivot;
    using System;

    public class DataModelTablePropertyConnectionNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para crear una tabla
            worksheet.Cells["A1"].PutValue("OrderID");
            worksheet.Cells["B1"].PutValue("Customer");
            worksheet.Cells["A2"].PutValue(1001);
            worksheet.Cells["B2"].PutValue("John Doe");
            worksheet.Cells["A3"].PutValue(1002);
            worksheet.Cells["B3"].PutValue("Jane Smith");

            // Crear un ListObject (tabla)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "OrdersTable";

            // Acceder al DataModelTable
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Mostrar el valor actual de ConnectionName
            Console.WriteLine("Current ConnectionName: " + dataModelTable.ConnectionName);

            // Crear una tabla dinámica usando la conexión de DataModelTable
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Customer");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "OrderID");

            // Nota: ConnectionName es de solo lectura, por lo que no podemos establecerla
            // Esto demuestra cómo usar el nombre de conexión existente
            if (!string.IsNullOrEmpty(dataModelTable.ConnectionName))
            {
                Console.WriteLine("This table is connected via: " + dataModelTable.ConnectionName);
            }

            // Guarda el libro de trabajo
            workbook.Save("DataModelTableConnectionNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


