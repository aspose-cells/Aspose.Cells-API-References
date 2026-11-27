---
title: "Cells.GetCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar Cell-elementet eller null på det angivna cellradindexet och kolumnindexet"
type: docs
url: /sv/net/aspose.cells/cells/getcell/
---
## Cells.GetCell method

Hämtar [`Cell`](../../cell/) elementet eller null på det angivna cellradindexet och kolumnindexet.

```csharp
[Obsolete("Use Cells.CheckCell(int row, int column) instead.")]
public Cell GetCell(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex |
| column | Int32 | Kolumnindex |

### Returvärde

Returnera Cell-objektet om ett Cell-objekt finns. Returnera null om cellen inte finns.

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället metoden CheckCell(int row, int column). Denna metod kommer att tas bort 12 månader senare från och med februari 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till cell på rad 1, kolumn 2 (0-baserat index)
            Cell cell = worksheet.Cells.GetCell(1, 2);
            
            // Ange värde och stil för demonstration
            cell.PutValue("Test Value");
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("GetCellDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


