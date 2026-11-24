---
title: "Cell.IsInArray"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt an, ob die Zellformel eine Array-Formel ist"
type: docs
url: /de/net/aspose.cells/cell/isinarray/
---
## Cell.IsInArray property

Gibt an, ob die Zellenformel eine Array‑Formel ist.

```csharp
[Obsolete("Use IsArrayFormula instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsInArray { get; }
```

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen Cell.IsArrayFormula, um zu prüfen, ob die Zellformel eine Array-Formel ist. Diese Eigenschaft wird 12 Monate nach Mai 2018 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsInArrayDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten mit Array-Formeln erstellen
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Setzen Sie eine Array-Formel mit der richtigen API
            worksheet.Cells["C2"].SetArrayFormula("A2:A3*B2:B3", 2, 1);

            // Überprüfen Sie die Eigenschaft IsInArray
            Cell cellInArray = worksheet.Cells["C2"];
            Cell cellNotInArray = worksheet.Cells["A2"];

            Console.WriteLine("Cell C2 is in array: " + cellInArray.IsInArray);
            Console.WriteLine("Cell A2 is in array: " + cellNotInArray.IsInArray);

            // Demonstrieren Sie das Löschen von Nicht-Array-Zellen
            for (int row = 1; row <= 3; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = worksheet.Cells[row, col];
                    if (!cell.IsInArray && !cell.IsFormula)
                    {
                        cell.PutValue("");
                    }
                }
            }

            // Speichere die Arbeitsmappe
            workbook.Save("IsInArrayDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


