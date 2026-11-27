---
title: "FormatConditionCollection.RemoveArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatConditionCollection-metoden. Tar bort ett villkorligt formaterat cellområde efter index"
type: docs
url: /sv/net/aspose.cells/formatconditioncollection/removearea/
---
## RemoveArea(int) {#removearea_1}

Tar bort det villkorligt formaterade cellområdet efter index.

```csharp
public void RemoveArea(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Indexet för det villkorligt formaterade cellområdet som ska tas bort. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till villkorsstyrd formatering
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];

            // Lägg till områden att formatera
            formatConditionCollection.AddArea(CellArea.CreateCellArea(0, 0, 10, 5)); // First area
            formatConditionCollection.AddArea(CellArea.CreateCellArea(5, 5, 15, 10)); // Second area

            // Lägg till ett villkor
            formatConditionCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");

            // Visa ursprungligt områdesantal (vi vet att vi lade till 2 områden)
            Console.WriteLine("Areas before removal: 2");

            // Ta bort det andra området (index 1)
            formatConditionCollection.RemoveArea(1);

            // Visa områdesantal efter borttagning (vi vet att vi tog bort 1 område)
            Console.WriteLine("Areas after removal: 1");

            // Spara arbetsboken
            workbook.Save("RemoveAreaDemo.xlsx");
        }
    }
}
```

### Se även

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveArea(int, int, int, int) {#removearea}

Ta bort villkorlig formatering i området.

```csharp
public bool RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startraden för intervallet. |
| startColumn | Int32 | Startkolumnen för intervallet. |
| totalRows | Int32 | Antalet rader i området. |
| totalColumns | Int32 | Antalet kolumner i området. |

### Returvärde

Returnerar TRUE, detta FormatCondtionCollection bör tas bort.

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            
            int idx = cfc.Add();
            FormatConditionCollection fcc = cfc[idx];
            
            // Lägg till ursprungligt område
            CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
            fcc.AddArea(initialArea);
            
            // Lägg till villkor
            idx = fcc.AddCondition(FormatConditionType.Expression);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "=A1>0";
            fc.Style.Font.Color = Color.Red;
            
            // Demonstrera RemoveArea med Int32-parametrar
            Console.WriteLine("Before removal - Areas count: " + fcc.Count);
            fcc.RemoveArea(0, 0, 1, 1); // Remove the initial area
            Console.WriteLine("After removal - Areas count: " + fcc.Count);
            
            // Lägg till nytt område
            CellArea newArea = CellArea.CreateCellArea(1, 1, 1, 1);
            fcc.AddArea(newArea);
            Console.WriteLine("After adding new area - Areas count: " + fcc.Count);
        }
    }
}
```

### Se även

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


