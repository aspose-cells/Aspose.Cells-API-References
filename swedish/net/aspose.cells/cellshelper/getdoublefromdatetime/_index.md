---
title: "CellsHelper.GetDoubleFromDateTime"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Konvertera datum och tid till ett dubbelvärde"
type: docs
url: /sv/net/aspose.cells/cellshelper/getdoublefromdatetime/
---
## CellsHelper.GetDoubleFromDateTime method

Konvertera datum‑tiden till dubbelvärde.

```csharp
public static double GetDoubleFromDateTime(DateTime dateTime, bool date1904)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dateTime | DateTime | Datum och tid. |
| date1904 | Boolean | 1904-datumsystem. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetDoubleFromDateTimeWithDateTimeBooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbokinstans
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta aktuellt datum och tid
            DateTime now = DateTime.Now;
            
            // Konvertera DateTime till dubbel med hjälp av CellsHelper
            double dateDouble = CellsHelper.GetDoubleFromDateTime(now, false);
            
            // Ange värdet i cell A1
            worksheet.Cells["A1"].PutValue(dateDouble);
            
            // Formatera cellen så att den visas som datum
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Number = 14; // Date format
            worksheet.Cells["A1"].SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("DateTimeConversionDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


