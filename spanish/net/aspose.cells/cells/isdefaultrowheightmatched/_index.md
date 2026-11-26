---
title: "Cells.IsDefaultRowHeightMatched"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Cells property. Indica que la altura de la fila y la altura de la fuente predeterminada coinciden"
type: docs
url: /es/net/aspose.cells/cells/isdefaultrowheightmatched/
---
## Cells.IsDefaultRowHeightMatched property

Indica que la altura de la fila y la altura de fuente predeterminada coinciden.

```csharp
public bool IsDefaultRowHeightMatched { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHeightMatchedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Establecer y demostrar la propiedad IsDefaultRowHeightMatched
            cells.IsDefaultRowHeightMatched = true;
            Console.WriteLine("IsDefaultRowHeightMatched: " + cells.IsDefaultRowHeightMatched);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");

            // Cargar el libro de trabajo guardado para verificar la propiedad
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;
            Console.WriteLine("Loaded IsDefaultRowHeightMatched: " + loadedCells.IsDefaultRowHeightMatched);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


