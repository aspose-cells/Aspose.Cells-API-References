---
title: "Cell.IsStyleSet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Indica se lo stile della cella è impostato. Se restituisce false significa che questa cella ha un formato predefinito"
type: docs
url: /it/net/aspose.cells/cell/isstyleset/
---
## Cell.IsStyleSet property

Indica se lo stile della cella è impostato. Se restituisce false, significa che questa cella ha un formato di cella predefinito.

```csharp
public bool IsStyleSet { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsStyleSetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Accedi a una cella che non è ancora stata stilizzata
            Cell unsetStyleCell = cells["A1"];
            Console.WriteLine($"Cell A1 IsStyleSet before styling: {unsetStyleCell.IsStyleSet}");

            // Stilizza una cella diversa
            Cell styledCell = cells["B2"];
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            styledCell.SetStyle(style);

            Console.WriteLine($"Cell B2 IsStyleSet after styling: {styledCell.IsStyleSet}");

            // Verifica se lo stile è ereditato dalla riga
            Row row = cells.Rows[4];
            row.SetStyle(style);
            Cell rowInheritedCell = cells["E4"];
            Console.WriteLine($"Cell E4 IsStyleSet (inherited from row): {rowInheritedCell.IsStyleSet}");

            // Imposta esplicitamente lo stile a null per una cella
            Cell nullStyleCell = cells["C3"];
            nullStyleCell.SetStyle(null);
            Console.WriteLine($"Cell C3 IsStyleSet after setting null: {nullStyleCell.IsStyleSet}");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


