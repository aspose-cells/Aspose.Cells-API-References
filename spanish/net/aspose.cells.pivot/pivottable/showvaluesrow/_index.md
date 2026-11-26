---
title: "PivotTable.ShowValuesRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Indica si se muestra la fila de valores"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showvaluesrow/
---
## PivotTable.ShowValuesRow property

Indica si se muestra la fila de valores.

```csharp
public bool ShowValuesRow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowValuesRowDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Configurar tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit as row
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity as data
            
            // Demostrar la propiedad ShowValuesRow
            Console.WriteLine("Initial ShowValuesRow: " + pivotTable.ShowValuesRow);
            pivotTable.ShowValuesRow = true;
            Console.WriteLine("After setting to true: " + pivotTable.ShowValuesRow);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableShowValuesRowDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


