---
title: "AutoFitterOptions.AutoFitMergedCells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoFitterOptions. Indica si se ajusta automáticamente la altura de la fila cuando las celdas están fusionadas en una fila. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/autofitteroptions/autofitmergedcells/
---
## AutoFitterOptions.AutoFitMergedCells property

Indica si se ajusta automáticamente la altura de la fila cuando las celdas están fusionadas en una fila. El valor predeterminado es false.

```csharp
[Obsolete("Use AutoFitterOptions.AutoFitMergedCellsType property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AutoFitMergedCells { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad AutoFitterOptions.AutoFitMergedCellsType. Esta propiedad será eliminada 12 meses después desde diciembre de 2018. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra y fusionar celdas
            worksheet.Cells["A1"].PutValue("This is a test of AutoFitMergedCells property");
            worksheet.Cells.Merge(0, 0, 3, 3); // Merge cells A1:C3

            // Crear AutoFitterOptions y establecer AutoFitMergedCells
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;

            // Ajustar automáticamente filas con celdas fusionadas
            worksheet.AutoFitRows(options);

            // Guarda el libro de trabajo
            workbook.Save("AutoFitMergedCellsExample.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


