---
title: "PivotTable.AutofitColumnWidthOnUpdate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si se ajusta automáticamente el ancho de columna al actualizar"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/
---
## PivotTable.AutofitColumnWidthOnUpdate property

Indica si se debe ajustar automáticamente el ancho de columna al actualizar.

```csharp
public bool AutofitColumnWidthOnUpdate { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAutofitColumnWidthOnUpdateDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Acceder a la hoja de cálculo que contiene la tabla dinámica
            Worksheet worksheet = workbook.Worksheets["PIVOT"];
            
            // Acceder a la tabla dinámica
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Desactivar ajuste automático del ancho de columna al actualizar
            pivotTable.AutofitColumnWidthOnUpdate = false;
            
            // Actualizar la tabla dinámica para aplicar los cambios
            worksheet.RefreshPivotTables();
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            Console.WriteLine("PivotTable AutofitColumnWidthOnUpdate property set successfully.");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


