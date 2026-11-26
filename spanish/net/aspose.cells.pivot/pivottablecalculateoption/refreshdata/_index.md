---
title: "PivotTableCalculateOption.RefreshData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTableCalculateOption. Indica si se actualiza la fuente de datos de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottablecalculateoption/refreshdata/
---
## PivotTableCalculateOption.RefreshData property

Indica si la fuente de datos de la tabla dinámica se actualiza.

```csharp
public bool RefreshData { get; set; }
```

### Observaciones

Si es verdadero, actualiza la caché de la tabla dinámica desde la fuente de datos, luego calcula todas las tablas dinámicas basándose en la misma caché.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyRefreshDataDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Configura datos de ejemplo para la tabla dinámica
            var cells = sheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("A");
            cells["B2"].PutValue(100);
            cells["A3"].PutValue("B");
            cells["B3"].PutValue(200);
            cells["A4"].PutValue("C");
            cells["B4"].PutValue(300);

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Modificar los datos de origen
            cells["B2"].PutValue(150); // Change value from 100 to 150

            // Calcula la tabla dinámica con la opción RefreshData
            PivotTableCalculateOption options = new PivotTableCalculateOption();
            options.RefreshData = true;
            pivotTable.CalculateData(options);

            // Muestra el valor actualizado de la tabla dinámica
            Console.WriteLine("Updated Pivot Table Value: " + cells["F5"].StringValue);
        }
    }
}
```

### Ver también

* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


