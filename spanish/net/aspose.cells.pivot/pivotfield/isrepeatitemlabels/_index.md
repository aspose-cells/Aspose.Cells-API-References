---
title: "PivotField.IsRepeatItemLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Indica si se deben repetir las etiquetas del campo en la región de fila o columna. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/isrepeatitemlabels/
---
## PivotField.IsRepeatItemLabels property

Indica si se deben repetir las etiquetas del campo en la región de fila o columna. El valor predeterminado es false.

```csharp
public bool IsRepeatItemLabels { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsRepeatItemLabelsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("example.xlsx");

            // Acceder a la hoja de cálculo que contiene la tabla dinámica
            Worksheet worksheet = workbook.Worksheets["Actual"];

            // Acceder a la tabla dinámica
            PivotTable pivotTable = worksheet.PivotTables[0];

            // Habilitar la repetición de etiquetas de elementos para el primer campo de fila
            pivotTable.RowFields[0].IsRepeatItemLabels = true;

            // Habilitar la repetición de etiquetas de elementos para el primer campo de columna
            pivotTable.ColumnFields[0].IsRepeatItemLabels = true;

            // Guardar el libro de trabajo modificado
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


