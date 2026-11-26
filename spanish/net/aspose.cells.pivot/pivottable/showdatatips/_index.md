---
title: "PivotTable.ShowDataTips"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "PivotTable property. Indica si los consejos emergentes deben mostrarse para las celdas de datos de PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showdatatips/
---
## PivotTable.ShowDataTips property

Indica si se deben mostrar descripciones emergentes para las celdas de datos de la tabla dinámica.

```csharp
public bool ShowDataTips { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowDataTipsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y algunos datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 20;

            // Crear una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Configurar tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Activar los consejos emergentes
            pivotTable.ShowDataTips = true;
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableWithDataTips.xlsx");
            
            Console.WriteLine("Pivot table with ShowDataTips enabled created successfully.");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


