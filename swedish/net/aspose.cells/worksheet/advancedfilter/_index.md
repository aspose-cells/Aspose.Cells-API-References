---
title: "Worksheet.AdvancedFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Arbetsbladmetod. Filtrerar data med komplexa kriterier"
type: docs
url: /sv/net/aspose.cells/worksheet/advancedfilter/
---
## Worksheet.AdvancedFilter method

Filtrerar data med komplexa kriterier.

```csharp
public void AdvancedFilter(bool isFilter, string listRange, string criteriaRange, string copyTo, 
    bool uniqueRecordOnly)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isFilter | Boolean | Anger om listan filtreras på plats. |
| listRange | String | Listintervallet. |
| criteriaRange | String | Kriterieintervallet. |
| copyTo | String | Intervallet dit data kopieras. |
| uniqueRecordOnly | Boolean | Endast visa eller kopiera unika rader. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAdvancedFilterWithBooleanStringStringStringBooleDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för filtrering
            // Rubriker
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["C1"].PutValue("Price");
            
            // Kriterier
            worksheet.Cells["A2"].PutValue("Product");
            worksheet.Cells["B2"].PutValue("Category");
            worksheet.Cells["C2"].PutValue("Fruits");
            
            // Data
            worksheet.Cells["A4"].PutValue("Apple");
            worksheet.Cells["B4"].PutValue("Fruits");
            worksheet.Cells["C4"].PutValue(2.5);
            
            worksheet.Cells["A5"].PutValue("Carrot");
            worksheet.Cells["B5"].PutValue("Vegetables");
            worksheet.Cells["C5"].PutValue(1.2);
            
            worksheet.Cells["A6"].PutValue("Banana");
            worksheet.Cells["B6"].PutValue("Fruits");
            worksheet.Cells["C6"].PutValue(1.8);

            // Tillämpa avancerat filter (filtrera på plats, endast unika poster)
            worksheet.AdvancedFilter(false, "A4:C6", "A1:C2", null, true);

            // Spara arbetsboken
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


