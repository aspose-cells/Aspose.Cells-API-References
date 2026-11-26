---
title: "PivotTableFormatCollection.FormatArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "PivotTableFormatCollection método. Formatea el área seleccionada"
type: docs
url: /es/net/aspose.cells.pivot/pivottableformatcollection/formatarea/
---
## PivotTableFormatCollection.FormatArea method

Formatea el área seleccionada.

```csharp
public PivotTableFormat FormatArea(PivotFieldType axisType, int fieldPosition, 
    PivotFieldSubtotalType subtotalType, PivotTableSelectionType selectionType, bool isGrandRow, 
    bool isGrandColumn, Style style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| axisType | PivotFieldType | La región de la PivotTable a la que se aplica esta regla. |
| fieldPosition | Int32 | Posición del campo dentro del eje al que se aplica esta regla. |
| subtotalType | PivotFieldSubtotalType | El tipo de filtro de subtotal del campo de tabla dinámica |
| selectionType | PivotTableSelectionType | Indica cómo seleccionar datos. |
| isGrandRow | Booleano | Indica si se están seleccionando filas de total general. |
| isGrandColumn | Booleano | Indica si se están seleccionando columnas de total general. |
| estilo | Estilo | El estilo que se aplica al área de la tabla dinámica. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionMethodFormatAreaWithPivotFieldTypeInt32PivotFieldSDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo fuente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Acceder a la tabla dinámica
            PivotTable pt = workbook.Worksheets["PIVOT_VBA_SUBTOTALS"].PivotTables[0];
            
            // Crear un estilo para formatear
            Style style = workbook.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Red);
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.LightGray;
            style.BackgroundColor = Color.LightGray;

            // Formatear el área de la tabla dinámica
            pt.PivotFormats.FormatArea(
                PivotFieldType.Row, 
                0, 
                PivotFieldSubtotalType.Automatic, 
                PivotTableSelectionType.DataAndLabel, 
                false, 
                false, 
                style);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTableFormat](../../pivottableformat/)
* enum [PivotFieldType](../../pivotfieldtype/)
* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* enum [PivotTableSelectionType](../../pivottableselectiontype/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


