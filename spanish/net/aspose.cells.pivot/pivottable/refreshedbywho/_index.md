---
title: "PivotTable.RefreshedByWho"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Obtiene el nombre del último usuario que actualizó esta PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/refreshedbywho/
---
## PivotTable.RefreshedByWho property

Obtiene el nombre del último usuario que actualizó esta tabla dinámica

```csharp
public string RefreshedByWho { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshedByWhoDemo
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

            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pt = sheet.PivotTables[pivotIndex];
            
            // Agregar campos a la tabla dinámica
            pt.AddFieldToArea(PivotFieldType.Row, 0);
            pt.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Actualizar la tabla dinámica para establecer la propiedad RefreshedByWho
            pt.RefreshData();
            pt.CalculateData();

            // Mostrar información de actualización
            Console.WriteLine("Pivot Table Refresh Information:");
            Console.WriteLine("Last Refresh Date: " + pt.RefreshDate);
            Console.WriteLine("Refreshed By: " + pt.RefreshedByWho);
            
            // Guardar y recargar para demostrar la persistencia de la propiedad
            string savePath = "PivotTableRefreshedByWhoDemo_Out.xlsx";
            wb.Save(savePath);
            
            // Recargar el libro y comprobar la propiedad
            Workbook wb2 = new Workbook(savePath);
            PivotTable pt2 = wb2.Worksheets[0].PivotTables[0];
            Console.WriteLine("\nAfter Reload:");
            Console.WriteLine("Last Refresh Date: " + pt2.RefreshDate);
            Console.WriteLine("Refreshed By: " + pt2.RefreshedByWho);
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


