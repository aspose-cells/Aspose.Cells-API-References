---
title: "HorizontalPageBreakCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HorizontalPageBreakCollection-metod. Lägger till ett horisontellt sidbryt i samlingen"
type: docs
url: /sv/net/aspose.cells/horizontalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Lägger till ett horisontellt sidbrytning i samlingen.

```csharp
public int Add(int row, int startColumn, int endColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex, nollbaserat. |
| startColumn | Int32 | Startkolumnindex, nollbaserad. |
| endColumn | Int32 | Slutkolumnindex, nollbaserad. |

### Returvärde

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Anmärkningar

Denna metod används för att lägga till en horisontell sidbrytning inom ett utskriftsområde.

### Exempel

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
            
            // Demonstrera Add-metoden med (Int32, Int32, Int32)-parametrar
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Se även

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Lägger till ett horisontellt sidbrytning i samlingen.

```csharp
public int Add(int row)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Cellens radindex, nollbaserat. |

### Returvärde

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Anmärkningar

Sidbrytning läggs till i cellens övre vänstra hörn. Vänligen ange ett horisontellt sidbryt och ett vertikalt sidbryt samtidigt.

### Exempel

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
            
            // Lägg till horisontella sidbrytningar med Int32-parameter
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Se även

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Lägger till ett horisontellt sidbrytning i samlingen.

```csharp
public int Add(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Cellens radindex, nollbaserat. |
| column | Int32 | Cellens kolumnindex, nollbaserat. |

### Returvärde

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Anmärkningar

Sidbrytning läggs till i cellens övre vänstra hörn. Vänligen ange ett horisontellt sidbryt och ett vertikalt sidbryt samtidigt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att skapa flera rader
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            // Lägg till horisontella sidbrytningar på specifika rader
            worksheet.HorizontalPageBreaks.Add(9, 0);  // Page break after row 9
            worksheet.HorizontalPageBreaks.Add(19, 0); // Page break after row 19
            worksheet.HorizontalPageBreaks.Add(29, 0); // Page break after row 29

            // Spara arbetsboken
            workbook.Save("HorizontalPageBreaksDemo.xlsx");
        }
    }
}
```

### Se även

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Lägger till ett horisontellt sidbrytning i samlingen.

```csharp
public int Add(string cellName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Cellnamn. |

### Returvärde

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Anmärkningar

Sidbrytning läggs till i cellens övre vänstra hörn. Vänligen ange ett horisontellt sidbryt och ett vertikalt sidbryt samtidigt.

### Exempel

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
            
            // Lägg till horisontell sidbrytning på rad 4 (D5 är rad 4 i nollbaserad index)
            worksheet.HorizontalPageBreaks.Add("D5");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


