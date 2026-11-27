---
title: "AutoFilter.ShowFilterButton"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-egenskap. Anger om AutoFilter-knappen för den här kolumnen är synlig"
type: docs
url: /sv/net/aspose.cells/autofilter/showfilterbutton/
---
## AutoFilter.ShowFilterButton property

Anger om AutoFilter-knappen för den här kolumnen är synlig.

```csharp
public bool ShowFilterButton { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyShowFilterButtonDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa ett listobjekt/tabell
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];

            // Aktivera autofilter och visa filterknappar
            table.AutoFilter.ShowFilterButton = true;

            // Spara arbetsboken
            workbook.Save("output_with_filter_buttons.xlsx");

            // Dölj filterknappar
            table.AutoFilter.ShowFilterButton = false;
            workbook.Save("output_without_filter_buttons.xlsx");
        }
    }
}
```

### Se även

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


