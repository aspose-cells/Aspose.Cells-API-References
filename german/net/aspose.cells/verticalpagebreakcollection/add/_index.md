---
title: "VerticalPageBreakCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Methode VerticalPageBreakCollection. Fügt der Sammlung einen vertikalen Seitenumbruch hinzu."
type: docs
url: /de/net/aspose.cells/verticalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Fügt einen vertikalen Seitenumbruch zur Sammlung hinzu.

```csharp
public int Add(int startRow, int endRow, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Startzeilenindex, nullbasiert. |
| endRow | Int32 | Endzeilenindex, nullbasiert. |
| column | Int32 | Spaltenindex, nullbasiert. |

### Rückgabewert

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Hinweise

Diese Methode wird verwendet, um einen vertikalen Seitenumbruch innerhalb eines Druckbereichs hinzuzufügen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;
            
            // Demonstrieren Sie Add mit den Parametern (Int32, Int32, Int32)
            verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
            
            // Zusätzliche Beispiele für den Kontext
            verticalPageBreaks.Add(4); // At column 4
            verticalPageBreaks.Add(5, 3); // At row 5, column 3

            Console.WriteLine("Vertical Page Breaks:");
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"{i}: StartRow={vpb.StartRow}, EndRow={vpb.EndRow}, Column={vpb.Column}");
            }

            workbook.Save("VerticalPageBreakDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Fügt einen vertikalen Seitenumbruch zur Sammlung hinzu.

```csharp
public int Add(int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Zellspaltenindex, nullbasiert. |

### Rückgabewert

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Hinweise

Der Seitenumbruch wird oben links in der Zelle hinzugefügt. Bitte setzen Sie gleichzeitig einen horizontalen und einen vertikalen Seitenumbruch.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Demonstrieren Sie die Add-Methode mit dem Int32-Parameter
            verticalPageBreaks.Add(4); // Add vertical page break at column 4

            // Geben Sie die Details des hinzugefügten Seitenumbruchs aus
            VerticalPageBreak vpb = verticalPageBreaks[0];
            Console.WriteLine($"Vertical Page Break: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");

            workbook.Save("VerticalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Fügt einen vertikalen Seitenumbruch zur Sammlung hinzu.

```csharp
public int Add(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zellzeilenindex, nullbasiert. |
| column | Int32 | Zellspaltenindex, nullbasiert. |

### Rückgabewert

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Hinweise

Der Seitenumbruch wird oben links in der Zelle hinzugefügt. Bitte setzen Sie gleichzeitig einen horizontalen und einen vertikalen Seitenumbruch.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rufen Sie die Sammlung der vertikalen Seitenumbrüche ab
            VerticalPageBreakCollection vPageBreaks = worksheet.VerticalPageBreaks;

            // Fügen Sie vertikale Seitenumbrüche an verschiedenen Spaltenpositionen hinzu
            vPageBreaks.Add(0, 5);  // Add page break after column 5
            vPageBreaks.Add(0, 10); // Add page break after column 10
            vPageBreaks.Add(0, 15); // Add page break after column 15

            // Fügen Sie einige Beispieldaten hinzu, um die Seitenumbrüche zu visualisieren
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[0, i].PutValue($"Column {i + 1}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("VerticalPageBreaksDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Fügt einen vertikalen Seitenumbruch zur Sammlung hinzu.

```csharp
public int Add(string cellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Zellname. |

### Rückgabewert

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Hinweise

Der Seitenumbruch wird oben links in der Zelle hinzugefügt. Bitte setzen Sie gleichzeitig einen horizontalen und einen vertikalen Seitenumbruch.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.VerticalPageBreaks.Add("G5");
            
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
    }
}
```

### Siehe auch

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


