---
title: "PivotTable.PrintTitles"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si los títulos de impresión para la hoja de cálculo se establecen en función del informe de la tabla dinámica. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/printtitles/
---
## PivotTable.PrintTitles property

Indica si los títulos de impresión para la hoja de cálculo se establecen en función del informe de la tabla dinámica. El valor predeterminado es false.

```csharp
public bool PrintTitles { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPrintTitlesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y algunos datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Configurar campos de la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Demostrar la propiedad PrintTitles
            pivotTable.PrintTitles = true;
            Console.WriteLine("PrintTitles set to: " + pivotTable.PrintTitles);

            // Guarda el libro de trabajo
            workbook.Save("PivotTablePrintTitlesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


