---
title: "Worksheet.HorizontalPageBreaks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene la colección HorizontalPageBreakCollection"
type: docs
url: /es/net/aspose.cells/worksheet/horizontalpagebreaks/
---
## Worksheet.HorizontalPageBreaks property

Obtiene la colección [`HorizontalPageBreakCollection`](../../horizontalpagebreakcollection/).

```csharp
public HorizontalPageBreakCollection HorizontalPageBreaks { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHorizontalPageBreaksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar saltos de página horizontales de diferentes maneras
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            worksheet.HorizontalPageBreaks.Add(15, 2);
            worksheet.HorizontalPageBreaks.Add("G5");

            // Eliminar el primer salto de página
            worksheet.HorizontalPageBreaks.RemoveAt(0);

            // Guardar salidas
            workbook.Save("HorizontalPageBreaksDemo.xlsx");
            workbook.Save("HorizontalPageBreaksDemo.pdf");
        }
    }
}
```

### Ver también

* class [HorizontalPageBreakCollection](../../horizontalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


