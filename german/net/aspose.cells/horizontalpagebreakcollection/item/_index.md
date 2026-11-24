---
title: "HorizontalPageBreakCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HorizontalPageBreakCollection-Eigenschaft. Gibt das HorizontalPageBreak-Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/horizontalpagebreakcollection/item/
---
## HorizontalPageBreakCollection indexer (1 of 2)

Gibt das [`HorizontalPageBreak`](../../horizontalpagebreak/) Element am angegebenen Index zurück.

```csharp
public HorizontalPageBreak this[int index] { get; }
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
    public class HorizontalPageBreakCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge horizontale Seitenumbrüche hinzu
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            // Greife auf Seitenumbrüche über die Item-Eigenschaft zu
            HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
            Console.WriteLine("First page break row: " + firstBreak.Row);
            
            // Modifiziere Zellen, die Seitenumbrüche beeinflussen
            worksheet.Cells.DeleteRows(0, 2);
            
            // Verifiziere, dass der Seitenumbruch angepasst wurde
            Console.WriteLine("First page break after row deletion: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### Siehe auch

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HorizontalPageBreakCollection indexer (2 of 2)

Gibt das [`HorizontalPageBreak`](../../horizontalpagebreak/) Element mit dem angegebenen Zellenamen zurück.

```csharp
public HorizontalPageBreak this[string cellName] { get; }
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
    using System;
    using Aspose.Cells;

    public class HorizontalPageBreakCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Füge ein paar horizontale Seitenumbrüche mit verschiedenen Überladungen hinzu
                worksheet.HorizontalPageBreaks.Add(5);          // break after row index 5
                worksheet.HorizontalPageBreaks.Add("D5");      // break at cell D5 (row index 4)

                // ----- Zugriff über ganzzahligen Index (Item[int]) -----
                // Die Item-Eigenschaft ist der Indexer, daher verwenden wir die []-Syntax
                HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
                Console.WriteLine("First break row (int index): " + firstBreak.Row);

                // ----- Zugriff über Zeichenketten-Schlüssel (Item[string]) -----
                // Rufe den Seitenumbruch ab, der mit dem Zellenamen "D5" hinzugefügt wurde
                HorizontalPageBreak breakByCell = worksheet.HorizontalPageBreaks["D5"];
                Console.WriteLine("Break added with \"D5\" is at row: " + breakByCell.Row);

                // Speichere die Arbeitsmappe, um zu überprüfen, dass die Seitenumbrüche gespeichert werden
                workbook.Save("HorizontalPageBreaks_ItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Siehe auch

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


