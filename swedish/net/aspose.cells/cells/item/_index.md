---
title: "Cells.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar Cell-elementet vid angivet cellradindex och kolumnindex"
type: docs
url: /sv/net/aspose.cells/cells/item/
---
## Cells indexer (1 of 2)

Hämtar [`Cell`](../../cell/) elementet vid angivet cellradindex och kolumnindex.

```csharp
public Cell this[int row, int column] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| row | Radindex. |
| column | Kolumnindex. |

### Returvärde

Objektet [`Cell`](../../cell/).

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Använda Item-egenskapen för att komma åt och ändra celler
            cells[0, 0].PutValue("Hello");
            cells[1, 0].PutValue("World");
            
            // Använda Style-egenskapen via Cells
            Style style1 = cells[0, 0].GetStyle();
            style1.Font.IsBold = true;
            cells[0, 0].SetStyle(style1);

            Style style2 = cells[1, 0].GetStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            cells[1, 0].SetStyle(style2);

            // Spara arbetsboken
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Cells indexer (2 of 2)

Hämtar [`Cell`](../../cell/) elementet vid det angivna cellnamnet.

```csharp
public Cell this[string cellName] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| cellName | Cellnamn, inklusive dess kolumnbokstav och radnummer, till exempel A5. |

### Returvärde

Ett [`Cell`](../../cell/) objekt

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till cellsamlingen
            Cells cells = worksheet.Cells;
            
            // Ställ in värden med Item-egenskapen
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            
            // Ställ in värden i ett område med Item-egenskapen
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);
            
            // Kom åt och ändra cellegenskaper med Item
            Cell cell = cells["B1"];
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


