---
title: "Enumeración PivotRefreshState"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Pivot.PivotRefreshState enum. El estado para actualizar tablas dinámicas"
type: docs
url: /es/net/aspose.cells.pivot/pivotrefreshstate/
---
## PivotRefreshState enumeration

El estado para actualizar las tablas dinámicas.

```csharp
public enum PivotRefreshState
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Success | `0` | Actualizado con éxito |
| UnsupportedExternalDataSource | `1` | La actualización falló porque la fuente de datos es externa. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotRefreshStateDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con una tabla dinámica de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Demostrar PivotRefreshState
            PivotRefreshState refreshState = pivotTable.RefreshData();
            if (refreshState == PivotRefreshState.Success)
            {
                Console.WriteLine("Pivot table refreshed successfully");
            }
            else if (refreshState == PivotRefreshState.UnsupportedExternalDataSource)
            {
                Console.WriteLine("External data source not supported - calculating data instead");
                pivotTable.CalculateData();
            }

            // Guarda el libro de trabajo
            workbook.Save("PivotRefreshStateDemo_out.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


