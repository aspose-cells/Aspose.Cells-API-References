---
title: "PivotTable.DisplayImmediateItems"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si los elementos en las áreas de filas y columnas son visibles cuando el área de datos de la PivotTable está vacía. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/displayimmediateitems/
---
## PivotTable.DisplayImmediateItems property

Indica si los elementos en las áreas de fila y columna son visibles cuando el área de datos de la PivotTable está vacía. El valor predeterminado es verdadero.

```csharp
public bool DisplayImmediateItems { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDisplayImmediateItemsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
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
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Demostrar la propiedad DisplayImmediateItems
            Console.WriteLine("Initial DisplayImmediateItems value: " + pivotTable.DisplayImmediateItems);
            
            // Cambiar el valor de la propiedad
            pivotTable.DisplayImmediateItems = false;
            Console.WriteLine("After setting to false: " + pivotTable.DisplayImmediateItems);

            // Guarda el libro de trabajo
            workbook.Save("PivotTableDisplayImmediateItemsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


