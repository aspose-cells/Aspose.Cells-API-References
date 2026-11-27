---
title: "Cells.Merge"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Slår ihop ett angivet cellområde till en enda cell"
type: docs
url: /sv/net/aspose.cells/cells/merge/
---
## Merge(int, int, int, int) {#merge}

Slår ihop ett angivet cellområde till en enda cell.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Första raden i detta område (nollbaserad) |
| firstColumn | Int32 | Första kolumnen i detta område (nollbaserad) |
| totalRows | Int32 | Antal rader (enbaserad) |
| totalColumns | Int32 | Antal kolumner (enbaserad) |

### Anmärkningar

Referera till den sammanslagna cellen via adressen för den övre vänstra cellen i området.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Sätt värden i celler för att demonstrera sammanslagning
            cells[0, 0].PutValue("Merged Area");
            cells[5, 5].PutValue("Not Merged");

            // Slå ihop celler med start i rad 0, kolumn 0 som sträcker sig över 3 rader och 2 kolumner
            cells.Merge(0, 0, 3, 2);

            // Spara arbetsboken
            workbook.Save("MergeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool) {#merge_1}

Slår ihop ett angivet cellområde till en enda cell.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool mergeConflict)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Första raden i detta område (nollbaserad) |
| firstColumn | Int32 | Första kolumnen i detta område (nollbaserad) |
| totalRows | Int32 | Antal rader (enbaserad) |
| totalColumns | Int32 | Antal kolumner (enbaserad) |
| mergeConflict | Boolean | Sammanfogningskonflikt för sammanslagna områden. |

### Anmärkningar

Referera till den sammanslagna cellen via adressen för den övre vänstra cellen i området. Om mergeConflict är true och det sammanslagna området krockar med andra sammanslagna celler, kommer de andra sammanslagna cellerna att tas bort automatiskt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Slå ihop celler från rad 3, kolumn 4 (D3) till rad 7, kolumn 5 (E7) - 5 rader och 2 kolumner
            worksheet.Cells.Merge(3, 4, 5, 2, true);
            
            // Spara arbetsboken
            workbook.Save("MergeDemoOutput.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool, bool) {#merge_2}

Slår ihop ett angivet cellområde till en enda cell.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool checkConflict, bool mergeConflict)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Första raden i detta område (nollbaserad) |
| firstColumn | Int32 | Första kolumnen i detta område (nollbaserad) |
| totalRows | Int32 | Antal rader (enbaserad) |
| totalColumns | Int32 | Antal kolumner (enbaserad) |
| checkConflict | Boolean | Anger om de sammanslagna cellerna intersectar andra sammanslagna celler |
| mergeConflict | Boolean | Sammanfogningskonflikt för sammanslagna områden. |

### Anmärkningar

Referera till den sammanslagna cellen via adressen för den övre vänstra cellen i området. Om mergeConflict är true och det sammanslagna området krockar med andra sammanslagna celler, kommer de andra sammanslagna cellerna att tas bort automatiskt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanBooDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Sätt in lite data i celler som ska slås ihop
            cells[0, 1].PutValue("Merged Cell");
            cells[1, 1].PutValue("This will be merged");

            // Slå ihop celler utan alternativ (enkel sammanslagning)
            cells.Merge(0, 1, 2, 2);
            Console.WriteLine("Cells merged without options");

            // Dela upp först för att demonstrera nästa sammanslagning
            cells.UnMerge(0, 1, 2, 2);

            // Slå ihop celler med ignoreStyle=false och mergeConflict=true
            cells.Merge(0, 1, 2, 2, false, true);
            Console.WriteLine("Cells merged with ignoreStyle=false and mergeConflict=true");

            // Spara arbetsboken
            workbook.Save("MergeCellsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


