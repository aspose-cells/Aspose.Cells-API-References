---
title: "Worksheet.MoveTo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Verschiebt das Blatt an eine andere Position in der Kalkulationstabelle"
type: docs
url: /de/net/aspose.cells/worksheet/moveto/
---
## Worksheet.MoveTo method

Verschiebt das Blatt an einen anderen Ort im Tabellenblatt.

```csharp
public void MoveTo(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Zielblatt-Index. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodMoveToWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Einige Arbeitsblätter hinzufügen
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Ein neues Arbeitsblatt hinzufügen und es an Position 1 verschieben
            Worksheet newWorksheet = workbook.Worksheets.Add("MovedSheet");
            newWorksheet.MoveTo(1);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


