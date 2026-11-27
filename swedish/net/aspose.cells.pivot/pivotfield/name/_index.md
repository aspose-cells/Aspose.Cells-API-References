---
title: "PivotField.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Representerar namnet på PivotField"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/name/
---
## PivotField.Name property

Representerar namnet på PivotField.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = new DateTime(2024, 1, 5);
            sheet.Cells["A3"].Value = new DateTime(2024, 1, 10);
            sheet.Cells["A4"].Value = new DateTime(2024, 2, 15);
            sheet.Cells["A5"].Value = new DateTime(2024, 3, 20);
            
            sheet.Cells["B1"].Value = "Value";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["B4"].Value = 300;
            sheet.Cells["B5"].Value = 400;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pt = sheet.PivotTables[index];
            
            // Lägg till radfält och demonstrera Name-egenskapen
            pt.AddFieldToArea(PivotFieldType.Row, 0);
            pt.RowFields[0].Name = "MyDateField";
            
            // Gruppera efter månader och år
            DateTime start = new DateTime(2024, 1, 1);
            DateTime end = new DateTime(2024, 12, 31);
            pt.RowFields[0].GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, true);
            
            // Skriv ut namnen på de grupperade fälten
            Console.WriteLine("Row Field 0 Name: " + pt.RowFields[0].Name); // Will show "MyYears"
            Console.WriteLine("Row Field 1 Name: " + pt.RowFields[1].Name); // Will show "MyMonths"
            
            // Spara arbetsboken
            wb.Save("PivotFieldNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


