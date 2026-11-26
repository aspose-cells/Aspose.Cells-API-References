---
title: "PivotTable.FormatRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "PivotTable method. Formatear los datos de la fila en el área de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/formatrow/
---
## PivotTable.FormatRow method

Da formato a los datos de fila en el área de la tabla dinámica

```csharp
public void FormatRow(int row, Style style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila del objeto Row |
| estilo | Estilo | Estilo que se debe formatear |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFormatRowWithInt32StyleDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // Datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Crear estilo para formatear
            Style style = wb.CreateStyle();
            style.Custom = "0.00%";
            style.Font.Name = "Calibri";
            style.Font.Size = 11;
            
            // Buscar y formatear filas
            Cell cell = worksheet.Cells.Find("A", null);
            if (cell != null)
            {
                pivotTable.FormatRow(cell.Row, style);
            }
            
            cell = worksheet.Cells.Find("B", null);
            if (cell != null)
            {
                pivotTable.FormatRow(cell.Row, style);
            }
            
            // Guarda el libro de trabajo
            wb.Save("PivotTableFormatRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


