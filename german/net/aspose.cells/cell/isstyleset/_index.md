---
title: "Cell.IsStyleSet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt an, ob der Stil der Zelle gesetzt ist. Wenn false zurückgegeben wird, bedeutet dies, dass diese Zelle das Standardzellenformat hat"
type: docs
url: /de/net/aspose.cells/cell/isstyleset/
---
## Cell.IsStyleSet property

Gibt an, ob der Zellenstil festgelegt ist. Wenn false zurückgegeben wird, bedeutet dies, dass diese Zelle ein Standardzellenformat hat.

```csharp
public bool IsStyleSet { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsStyleSetDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Greifen Sie auf eine Zelle zu, die noch nicht gestylt wurde
            Cell unsetStyleCell = cells["A1"];
            Console.WriteLine($"Cell A1 IsStyleSet before styling: {unsetStyleCell.IsStyleSet}");

            // Stylen Sie eine andere Zelle
            Cell styledCell = cells["B2"];
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            styledCell.SetStyle(style);

            Console.WriteLine($"Cell B2 IsStyleSet after styling: {styledCell.IsStyleSet}");

            // Überprüfen Sie, ob der Stil von der Zeile geerbt wird
            Row row = cells.Rows[4];
            row.SetStyle(style);
            Cell rowInheritedCell = cells["E4"];
            Console.WriteLine($"Cell E4 IsStyleSet (inherited from row): {rowInheritedCell.IsStyleSet}");

            // Setzen Sie den Stil einer Zelle explizit auf null
            Cell nullStyleCell = cells["C3"];
            nullStyleCell.SetStyle(null);
            Console.WriteLine($"Cell C3 IsStyleSet after setting null: {nullStyleCell.IsStyleSet}");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


