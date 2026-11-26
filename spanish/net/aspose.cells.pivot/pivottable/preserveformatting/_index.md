---
title: "PivotTable.PreserveFormatting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si el formato de celda PivotTableFormat se conserva cuando la PivotTable se actualiza o recalcula"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/preserveformatting/
---
## PivotTable.PreserveFormatting property

Indica si el formato de celda ([`PivotTableFormat`](../../pivottableformat/)) se conserva cuando la PivotTable se actualiza o recalcula.

```csharp
[Obsolete("Use PivotTable.PreserveCellFormattingOnUpdate property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PreserveFormatting { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotTable.PreserveCellFormattingOnUpdate. Este método será eliminado 12 meses después desde julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("source.xlsx");
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accede a la primera tabla dinámica
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Habilitar la preservación del formato durante la actualización
            pivotTable.PreserveFormatting = true;
            
            // Aplicar algo de formato al área de datos de la tabla dinámica
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // Formatear el área de datos de la tabla dinámica
            pivotTable.FormatAll(style);
            
            // Actualizar y calcular los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


