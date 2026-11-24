---
title: "Style.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Methode. Bestimmt, ob zwei Style‑Instanzen gleich sind"
type: docs
url: /de/net/aspose.cells/style/equals/
---
## Style.Equals method

Bestimmt, ob zwei Style-Instanzen gleich sind.

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object | Das Style‑Objekt, das mit dem aktuellen Style‑Objekt verglichen werden soll. |

### Rückgabewert

true, wenn das angegebene Objekt dem aktuellen Objekt gleich ist; andernfalls false.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie zwei Stile zum Vergleich
            Style style1 = workbook.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            style1.HorizontalAlignment = TextAlignmentType.Center;

            Style style2 = workbook.CreateStyle();
            style2.Font.Name = "Arial";
            style2.Font.Size = 12;
            style2.HorizontalAlignment = TextAlignmentType.Center;

            try
            {
                // Rufen Sie die Equals‑Methode auf, um die Stile zu vergleichen
                bool areEqual = style1.Equals((object)style2);

                // Ergebnis anzeigen
                Console.WriteLine($"The styles are equal: {areEqual}");

                // Wenden Sie die Stile an, um zu zeigen, dass sie identisch sind
                if (areEqual)
                {
                    Cell cell1 = worksheet.Cells["A1"];
                    cell1.PutValue("Style 1");
                    cell1.SetStyle(style1);

                    Cell cell2 = worksheet.Cells["A2"];
                    cell2.PutValue("Style 2");
                    cell2.SetStyle(style2);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("StyleEqualsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


