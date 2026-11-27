---
title: "Enum FilterOperatorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FilterOperatorType-enum. Anpassad filteroperatortyp"
type: docs
url: /sv/net/aspose.cells/filteroperatortype/
---
## FilterOperatorType enumeration

Anpassad filteroperatortyp.

```csharp
public enum FilterOperatorType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| LessOrEqual | `0` | Representerar LessOrEqual-operatorn. |
| LessThan | `1` | Representerar LessThan-operatorn. |
| Equal | `2` | Representerar lika-operatorn. |
| GreaterThan | `3` | Representerar större än-operatorn. |
| NotEqual | `4` | Representerar inte lika-operatorn. |
| GreaterOrEqual | `5` | Representerar större än eller lika med-operatorn. |
| None | `6` | Representerar ingen jämförelse. |
| BeginsWith | `7` | Börjar med texten. |
| EndsWith | `8` | Slutar med texten. |
| Contains | `9` | Innehåller texten. |
| NotContains | `10` | Innehåller inte texten. |
| NotBeginsWith | `11` | Börjar inte med texten. |
| NotEndsWith | `12` | Slutar inte med texten. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFilterOperatorTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Names");
            worksheet.Cells["A2"].PutValue("Bob");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["A4"].PutValue("Bobby");
            worksheet.Cells["A5"].PutValue("Tom");
            
            // Ställ in auto-filterintervall
            worksheet.AutoFilter.Range = "A1:A5";
            
            // Applicera anpassat filter för att visa namn som börjar med "Bo"
            worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "Bo");
            
            // Uppdatera filtret
            worksheet.AutoFilter.Refresh();
            
            // Spara arbetsboken
            workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


