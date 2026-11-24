---
title: "HorizontalPageBreakCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HorizontalPageBreakCollection-Methode. Fügt der Sammlung einen horizontalen Seitenumbruch hinzu"
type: docs
url: /de/net/aspose.cells/horizontalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Fügt der Sammlung einen horizontalen Seitenumbruch hinzu.

```csharp
public int Add(int row, int startColumn, int endColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex, nullbasiert. |
| startColumn | Int32 | Startspaltenindex, nullbasiert. |
| endColumn | Int32 | Endspaltenindex, nullbasiert. |

### Rückgabewert

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Hinweise

Diese Methode wird verwendet, um innerhalb eines Druckbereichs einen horizontalen Seitenumbruch hinzuzufügen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Demonstriere die Add-Methode mit (Int32, Int32, Int32)-Parametern
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Fügt der Sammlung einen horizontalen Seitenumbruch hinzu.

```csharp
public int Add(int row)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zellzeilenindex, nullbasiert. |

### Rückgabewert

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Hinweise

Der Seitenumbruch wird oben links in der Zelle hinzugefügt. Bitte setzen Sie gleichzeitig einen horizontalen und einen vertikalen Seitenumbruch.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge horizontale Seitenumbrüche mit dem Int32-Parameter hinzu
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Fügt der Sammlung einen horizontalen Seitenumbruch hinzu.

```csharp
public int Add(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zellzeilenindex, nullbasiert. |
| column | Int32 | Zellspaltenindex, nullbasiert. |

### Rückgabewert

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Hinweise

Der Seitenumbruch wird oben links in der Zelle hinzugefügt. Bitte setzen Sie gleichzeitig einen horizontalen und einen vertikalen Seitenumbruch.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten hinzu, um mehrere Zeilen zu erstellen
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            // Füge horizontale Seitenumbrüche in bestimmten Zeilen ein
            worksheet.HorizontalPageBreaks.Add(9, 0);  // Page break after row 9
            worksheet.HorizontalPageBreaks.Add(19, 0); // Page break after row 19
            worksheet.HorizontalPageBreaks.Add(29, 0); // Page break after row 29

            // Speichere die Arbeitsmappe
            workbook.Save("HorizontalPageBreaksDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Fügt der Sammlung einen horizontalen Seitenumbruch hinzu.

```csharp
public int Add(string cellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Zellname. |

### Rückgabewert

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Hinweise

Der Seitenumbruch wird oben links in der Zelle hinzugefügt. Bitte setzen Sie gleichzeitig einen horizontalen und einen vertikalen Seitenumbruch.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einen horizontalen Seitenumbruch in Zeile 4 ein (D5 ist Zeile 4 im nullbasierten Index)
            worksheet.HorizontalPageBreaks.Add("D5");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


