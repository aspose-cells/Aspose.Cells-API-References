---
title: "PivotTable.PivotFormats"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Obtiene todos los formatos de celda aplicados a esta tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/pivotformats/
---
## PivotTable.PivotFormats property

Obtiene todos los formatos de celda aplicados a esta tabla dinámica.

```csharp
public PivotTableFormatCollection PivotFormats { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPivotFormatsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B4"].Value = 20;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Crear estilo para formatear
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.LightBlue;
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, System.Drawing.Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, System.Drawing.Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, System.Drawing.Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, System.Drawing.Color.Black);

            // Aplicar formato al área de datos de la tabla dinámica
            pivotTable.PivotFormats.FormatArea(
                PivotFieldType.Data, 
                0, 
                PivotFieldSubtotalType.None, 
                PivotTableSelectionType.DataAndLabel, 
                false, 
                false, 
                style);

            // Guarda el libro de trabajo
            workbook.Save("PivotTableWithFormats.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTableFormatCollection](../../pivottableformatcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


