---
title: "Style.HasBorders"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Verifica se sono stati impostati bordi per lo stile"
type: docs
url: /it/net/aspose.cells/style/hasborders/
---
## Style.HasBorders property

Verifica se sono stati impostati bordi per lo stile.

```csharp
public bool HasBorders { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyHasBordersDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Accedi alla cella A1 e verifica se ha bordi (dovrebbe essere false per impostazione predefinita)
            Cell cellA1 = cells["A1"];
            Console.WriteLine("Cell A1 has borders: " + cellA1.GetStyle().HasBorders);

            // Crea uno stile con bordi
            Style styleWithBorders = workbook.CreateStyle();
            styleWithBorders.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            styleWithBorders.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // Applica lo stile alla cella B1
            Cell cellB1 = cells["B1"];
            cellB1.SetStyle(styleWithBorders);

            // Verifica se la cella B1 ha bordi (dovrebbe essere true ora)
            Console.WriteLine("Cell B1 has borders: " + cellB1.GetStyle().HasBorders);

            // Salva la cartella di lavoro
            workbook.Save("HasBordersDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


