---
title: "AutoFilter.AddFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Lägger till ett filter för en filterkolumn"
type: docs
url: /sv/net/aspose.cells/autofilter/addfilter/
---
## AutoFilter.AddFilter method

Lägger till ett filter för en filterkolumn.

```csharp
public void AddFilter(int fieldIndex, string criteria)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstra fältet är fält 0). |
| kriterier | String | Det angivna kriteriet (en sträng; till exempel "101"). Det kan endast vara null eller vara ett av cellernas värden i den här kolumnen. |

### Anmärkningar

MS Excel 2007 stöder flera val i en filterkolumn.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFilterWithInt32StringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["A5"].PutValue("Date");
            worksheet.Cells["A6"].PutValue("Elderberry");
            
            // Skapa autofilterområde
            worksheet.AutoFilter.Range = "A1:A6";
            
            // Hämta autofiltret
            AutoFilter filter = worksheet.AutoFilter;
            
            // Lägg till filter för värden som börjar med 'A' och 'E'
            filter.AddFilter(0, "A*");
            filter.AddFilter(0, "E*");
            
            // Uppdatera filtret
            filter.Refresh();
            
            // Spara arbetsboken
            workbook.Save("AutoFilterAddFilterDemo.xlsx");
        }
    }
}
```

### Se även

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


