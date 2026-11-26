---
title: "PivotTableFormat.PivotArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTableFormat. Obtiene el área de tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottableformat/pivotarea/
---
## PivotTableFormat.PivotArea property

Obtiene el área de la tabla dinámica.

```csharp
public PivotArea PivotArea { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableFormatPropertyPivotAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);

            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Agregue campos a áreas pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Obtenga el formato de tabla dinámica y configure su área de tabla dinámica
            int formatIndex = pivotTable.PivotFormats.Add();
            PivotTableFormat pivotFormat = pivotTable.PivotFormats[formatIndex];
            PivotArea pivotArea = pivotFormat.PivotArea;
            
            // Establezca las propiedades del área de tabla dinámica
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;

            // Cree y aplique un estilo al área de tabla dinámica
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            pivotFormat.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("PivotTableWithPivotArea.xlsx");
        }
    }
}
```

### Ver también

* class [PivotArea](../../pivotarea/)
* class [PivotTableFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


