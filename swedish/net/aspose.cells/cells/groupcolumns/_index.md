---
title: "Cells.GroupColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Grupperar kolumner"
type: docs
url: /sv/net/aspose.cells/cells/groupcolumns/
---
## GroupColumns(int, int) {#groupcolumns}

Grupperar kolumner.

```csharp
public void GroupColumns(int firstIndex, int lastIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | Int32 | Det första kolumnindexet som ska grupperas. |
| lastIndex | Int32 | Det sista kolumnindexet som ska grupperas. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Gruppera kolumner från index 0 till 255
            cells.GroupColumns(0, 255);

            // Spara arbetsboken
            string outputPath = "outputGroupColumns.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Columns grouped successfully. File saved to: " + outputPath);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupColumns(int, int, bool) {#groupcolumns_1}

Grupperar kolumner.

```csharp
public void GroupColumns(int firstIndex, int lastIndex, bool isHidden)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | Int32 | Det första kolumnindexet som ska grupperas. |
| lastIndex | Int32 | Det sista kolumnindexet som ska grupperas. |
| isHidden | Boolean | Anger om de grupperade kolumnerna är dolda. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Gruppera kolumner 5 till 7 (3 kolumner) och dölj dem
            cells.GroupColumns(5, 7, true);

            // Spara arbetsboken
            workbook.Save("GroupColumnsOutput.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


