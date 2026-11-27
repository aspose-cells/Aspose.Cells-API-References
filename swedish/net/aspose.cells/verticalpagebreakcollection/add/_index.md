---
title: "VerticalPageBreakCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VerticalPageBreakCollection-metoden. Lägger till ett vertikalt sidbryt i samlingen"
type: docs
url: /sv/net/aspose.cells/verticalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Lägger till ett vertikalt sidbrytning i samlingen.

```csharp
public int Add(int startRow, int endRow, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startradens index, nollbaserat. |
| endRow | Int32 | Slutradens index, nollbaserat. |
| column | Int32 | Kolumnindex, nollbaserat. |

### Returvärde

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Anmärkningar

Denna metod används för att lägga till ett vertikalt sidbryt inom ett utskriftsområde.

### Exempel

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
            
            // Demonstrera Add med parametrarna (Int32, Int32, Int32)
            verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
            
            // Ytterligare exempel för kontext
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

### Se även

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Lägger till ett vertikalt sidbrytning i samlingen.

```csharp
public int Add(int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Cellens kolumnindex, nollbaserat. |

### Returvärde

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Anmärkningar

Sidbrytning läggs till i cellens övre vänstra hörn. Vänligen ange ett horisontellt sidbryt och ett vertikalt sidbryt samtidigt.

### Exempel

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

            // Demonstrera Add-metoden med Int32-parameter
            verticalPageBreaks.Add(4); // Add vertical page break at column 4

            // Skriv ut detaljerna för den tillagda sidbrytningen
            VerticalPageBreak vpb = verticalPageBreaks[0];
            Console.WriteLine($"Vertical Page Break: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");

            workbook.Save("VerticalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### Se även

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Lägger till ett vertikalt sidbrytning i samlingen.

```csharp
public int Add(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Cellens radindex, nollbaserat. |
| column | Int32 | Cellens kolumnindex, nollbaserat. |

### Returvärde

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Anmärkningar

Sidbrytning läggs till i cellens övre vänstra hörn. Vänligen ange ett horisontellt sidbryt och ett vertikalt sidbryt samtidigt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta samlingen av vertikala sidbrytningar
            VerticalPageBreakCollection vPageBreaks = worksheet.VerticalPageBreaks;

            // Lägg till vertikala sidbrytningar på olika kolumnpositioner
            vPageBreaks.Add(0, 5);  // Add page break after column 5
            vPageBreaks.Add(0, 10); // Add page break after column 10
            vPageBreaks.Add(0, 15); // Add page break after column 15

            // Lägg till lite exempeldata för att visualisera sidbrytningarna
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[0, i].PutValue($"Column {i + 1}");
            }

            // Spara arbetsboken
            workbook.Save("VerticalPageBreaksDemo.xlsx");
        }
    }
}
```

### Se även

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Lägger till ett vertikalt sidbrytning i samlingen.

```csharp
public int Add(string cellName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Cellnamn. |

### Returvärde

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Anmärkningar

Sidbrytning läggs till i cellens övre vänstra hörn. Vänligen ange ett horisontellt sidbryt och ett vertikalt sidbryt samtidigt.

### Exempel

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

### Se även

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


