---
title: "PivotTable.RefreshDate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Obtiene la última fecha y hora en que se actualizó la PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/refreshdate/
---
## PivotTable.RefreshDate property

Obtiene la fecha y hora de la última actualización de la tabla dinámica.

```csharp
public DateTime RefreshDate { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshDateDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 8;

            // Agregar una tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pt = sheet.PivotTables[index];
            
            // Actualiza la tabla dinámica para establecer la fecha de actualización
            pt.RefreshData();
            pt.CalculateData();

            // Mostrar información de la fecha de actualización
            Console.WriteLine("Pivot Table Refresh Date: " + pt.RefreshDate.ToLongDateString());
            Console.WriteLine("Refreshed By: " + pt.RefreshedByWho);

            // Guarde y vuelva a cargar para demostrar la persistencia
            string savePath = "PivotTableRefreshDateDemo_Out.xlsx";
            wb.Save(savePath);
            
            // Recargar y mostrar la fecha de actualización nuevamente
            Workbook wb2 = new Workbook(savePath);
            PivotTable pt2 = wb2.Worksheets[0].PivotTables[0];
            Console.WriteLine("\nAfter reloading:");
            Console.WriteLine("Pivot Table Refresh Date: " + pt2.RefreshDate.ToLongDateString());
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


