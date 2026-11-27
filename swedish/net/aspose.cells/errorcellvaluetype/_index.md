---
title: "Enum ErrorCellValueType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ErrorCellValueType enum. Representerar ett cellvärde som innehåller ett fel"
type: docs
url: /sv/net/aspose.cells/errorcellvaluetype/
---
## ErrorCellValueType enumeration

Representerar ett cellvärde som innehåller ett fel.

```csharp
public enum ErrorCellValueType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Value | `1` | Representerar värdet i en cell som innehåller ett #VALUE!-fel. |
| Ref | `3` | Representerar värdet i en cell som innehåller ett #REF!-fel. |
| Name | `4` | Representerar värdet i en cell som innehåller ett #NAME?-fel. |
| NA | `6` | Representerar värdet i en cell som innehåller ett #N/A-fel. |
| Blocked | `10` | Representerar värdet i en cell som innehåller ett #BLOCKED!-fel. |
| Busy | `14` | Representerar värdet i en cell som innehåller ett #BUSY!-fel. |
| Calc | `13` | Representerar värdet i en cell som innehåller ett #CALC!-fel. |
| Connect | `9` | Representerar värdet i en cell som innehåller ett #CONNECT!-fel. |
| Field | `12` | Representerar värdet i en cell som innehåller ett #FIELD!-fel. |
| Spill | `8` | Representerar värdet i en cell som innehåller ett #SPILL!-fel. |
| Unknown | `11` | Representerar värdet i en cell som innehåller ett #UNKNOWN!-fel. |
| TimeOut | `19` | Representerar värdet i en cell som innehåller ett #TIMEOUT!-fel. |
| External | `18` | Representerar värdet i en cell som innehåller ett #EXTERNAL!-fel. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassErrorCellValueTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in en formel som ger ett spill-fel.
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3;1,2,3})";
            
            try
            {
                // Beräkna formler för att utlösa felet.
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // Förväntat spill-fel
            }
            
            // Hämta cellens rika värde
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // Kontrollera feltypen
            if (richValue.ErrorValue == ErrorCellValueType.Spill)
            {
                Console.WriteLine("Cell contains a spill error as expected");
            }
            
            // Spara arbetsboken
            workbook.Save("ErrorCellValueTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


