---
title: "WorksheetCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Hämtar Worksheet-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/item/
---
## WorksheetCollection indexer (1 of 2)

Hämtar [`Worksheet`](../../worksheet/) elementet på det angivna indexet.

```csharp
public Worksheet this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Använder Item-egenskapen för att komma åt cell
            Cell cell = cells[0, 0];
            cell.Formula = "=SUM(1, 2, 3)";
            
            workbook.CalculateFormula();
            Console.WriteLine("Cell value: " + cell.IntValue);
        }
    }
}
```

### Se även

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorksheetCollection indexer (2 of 2)

Hämtar [`Worksheet`](../../worksheet/) elementet med det angivna namnet.

```csharp
public Worksheet this[string sheetName] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| sheetName | Arbetsbladsnamn |

### Returvärde

Elementet med det angivna namnet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt kalkylblad med Item-egenskapen via index och namn
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            
            // Kom åt kalkylblad via namn med Item-egenskapen
            Worksheet accessedSheet = workbook.Worksheets["FirstSheet"];
            
            // Lägg till data för att demonstrera åtkomst till kalkylblad
            Cells cells = accessedSheet.Cells;
            cells["A1"].PutValue("Worksheet accessed successfully!");
            cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Infoga en kolumn i det andra bladet
            workbook.Worksheets["SecondSheet"].Cells.InsertColumn(1);
            
            // Spara arbetsboken
            workbook.Save("WorksheetCollectionItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


