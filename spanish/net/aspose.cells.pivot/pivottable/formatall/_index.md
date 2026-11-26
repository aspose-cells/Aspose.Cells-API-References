---
title: "PivotTable.FormatAll"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTable. Formatea todas las celdas en el área de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/formatall/
---
## PivotTable.FormatAll method

Da formato a todas las celdas en el área de la tabla dinámica

```csharp
public void FormatAll(Style style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo | Estilo que se debe formatear |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFormatAllWithStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            var cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;
            
            // Crear tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Crear y configurar estilo
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;
            
            // Aplicar estilo a toda la tabla dinámica
            pivotTable.FormatAll(style);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableFormatAllDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


