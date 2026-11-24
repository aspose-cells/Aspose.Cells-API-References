---
title: "LineFormat.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LineFormat-Methode. Bestimmt, ob diese Instanz denselben Wert wie ein anderer angegebener LineFormat-Objekt hat."
type: docs
url: /de/net/aspose.cells.drawing/lineformat/equals/
---
## LineFormat.Equals method

Bestimmt, ob diese Instanz denselben Wert wie ein anderer angegebener [`LineFormat`](../)-Objekt hat.

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object | Das [`LineFormat`](../)-Objekt, das mit dieser Instanz verglichen werden soll. |

### Rückgabewert

true, wenn der Wert des obj-Parameters dem Wert dieser Instanz entspricht; andernfalls false. Wenn obj null ist, gibt diese Methode false zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge dem Arbeitsblatt eine Linienform hinzu
            worksheet.Shapes.AddLine(1, 1, 10, 10, 100, 0);
            
            // Holen Sie das Linienformat der ersten Form
            LineFormat lineFmt1 = worksheet.Shapes[0].Line;
            LineFormat lineFmt2 = worksheet.Shapes[0].Line;
            
            // Vergleichen Sie die Linienformate mit der Equals-Methode
            if (lineFmt1.Equals((object)lineFmt2))
            {
                Console.WriteLine("The line formats are equal.");
            }
            else
            {
                Console.WriteLine("The line formats are not equal.");
            }
        }
    }
}
```

### Siehe auch

* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


