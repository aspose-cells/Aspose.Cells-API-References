---
title: "Cell.IsStyleSet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Indica si el estilo de la celda está establecido. Si devuelve false, significa que esta celda tiene un formato de celda predeterminado"
type: docs
url: /es/net/aspose.cells/cell/isstyleset/
---
## Cell.IsStyleSet property

Indica si el estilo de la celda está establecido. Si devuelve false, significa que esta celda tiene un formato de celda predeterminado.

```csharp
public bool IsStyleSet { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsStyleSetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Acceda a una celda que aún no ha sido estilizada
            Cell unsetStyleCell = cells["A1"];
            Console.WriteLine($"Cell A1 IsStyleSet before styling: {unsetStyleCell.IsStyleSet}");

            // Estilice una celda diferente
            Cell styledCell = cells["B2"];
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            styledCell.SetStyle(style);

            Console.WriteLine($"Cell B2 IsStyleSet after styling: {styledCell.IsStyleSet}");

            // Compruebe si el estilo se hereda de la fila
            Row row = cells.Rows[4];
            row.SetStyle(style);
            Cell rowInheritedCell = cells["E4"];
            Console.WriteLine($"Cell E4 IsStyleSet (inherited from row): {rowInheritedCell.IsStyleSet}");

            // Establecer explícitamente el estilo a null para una celda
            Cell nullStyleCell = cells["C3"];
            nullStyleCell.SetStyle(null);
            Console.WriteLine($"Cell C3 IsStyleSet after setting null: {nullStyleCell.IsStyleSet}");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


