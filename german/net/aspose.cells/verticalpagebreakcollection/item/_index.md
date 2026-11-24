---
title: "VerticalPageBreakCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VerticalPageBreakCollection-Eigenschaft. Gibt das VerticalPageBreak-Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/verticalpagebreakcollection/item/
---
## VerticalPageBreakCollection indexer (1 of 2)

Gibt das [`VerticalPageBreak`](../../verticalpagebreak/) Element am angegebenen Index zurück.

```csharp
public VerticalPageBreak this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Vertikale Seitenumbrüche hinzufügen
            worksheet.VerticalPageBreaks.Add(5);
            worksheet.VerticalPageBreaks.Add(10);
            worksheet.VerticalPageBreaks.Add(15);

            // Zugriff auf und Anzeige von Seitenumbrüchen über die Item‑Eigenschaft
            VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;
            Console.WriteLine("Vertical Page Breaks:");
            for (int i = 0; i < vpagebreaks.Count; i++)
            {
                Console.WriteLine($"Break {i + 1}: Column = {vpagebreaks[i].Column}");
            }

            // Entfernen und erneut hinzufügen, um einen Seitenumbruch zu ändern, da Column schreibgeschützt ist
            int column = vpagebreaks[1].Column;
            vpagebreaks.RemoveAt(1);
            vpagebreaks.Add(12);
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine($"Break 2: Column = {vpagebreaks[1].Column}");
        }
    }
}
```

### Siehe auch

* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## VerticalPageBreakCollection indexer (2 of 2)

Gibt das [`VerticalPageBreak`](../../verticalpagebreak/) Element mit dem angegebenen Zellnamen zurück.

```csharp
public VerticalPageBreak this[string cellName] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| cellName | Zellname. |

### Rückgabewert

Das Element mit dem angegebenen Zellnamen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige vertikale Seitenumbrüche hinzu
            worksheet.VerticalPageBreaks.Add(3);
            worksheet.VerticalPageBreaks.Add(7);

            try
            {
                // Greife auf die VerticalPageBreakCollection zu
                VerticalPageBreakCollection pageBreaks = worksheet.VerticalPageBreaks;

                // Demonstriere den Zugriff auf Elemente über die Item‑Eigenschaft (Indexer)
                Console.WriteLine("Vertical Page Breaks in the worksheet:");
                for (int i = 0; i < pageBreaks.Count; i++)
                {
                    VerticalPageBreak vpb = pageBreaks[i];
                    Console.WriteLine($"Break {i + 1}: Column = {vpb.Column}, StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("VerticalPageBreakItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


