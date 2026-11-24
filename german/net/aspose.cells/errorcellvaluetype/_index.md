---
title: "Enum ErrorCellValueType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ErrorCellValueType Aufzählung. Stellt einen Zellenwert dar, der einen Fehler enthält"
type: docs
url: /de/net/aspose.cells/errorcellvaluetype/
---
## ErrorCellValueType enumeration

Stellt einen Zellenwert dar, der einen Fehler enthält.

```csharp
public enum ErrorCellValueType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Value | `1` | Stellt den Wert einer Zelle dar, die einen #VALUE!-Fehler enthält. |
| Ref | `3` | Stellt den Wert einer Zelle dar, die einen #REF!-Fehler enthält. |
| Name | `4` | Stellt den Wert einer Zelle dar, die einen #NAME?-Fehler enthält. |
| NA | `6` | Stellt den Wert einer Zelle dar, die einen #N/A-Fehler enthält. |
| Blocked | `10` | Stellt den Wert einer Zelle dar, die einen #BLOCKED!-Fehler enthält. |
| Busy | `14` | Stellt den Wert einer Zelle dar, die einen #BUSY!-Fehler enthält. |
| Calc | `13` | Stellt den Wert einer Zelle dar, die einen #CALC!-Fehler enthält. |
| Connect | `9` | Stellt den Wert einer Zelle dar, die einen #CONNECT!-Fehler enthält. |
| Field | `12` | Stellt den Wert einer Zelle dar, die einen #FIELD!-Fehler enthält. |
| Spill | `8` | Stellt den Wert einer Zelle dar, die einen #SPILL!-Fehler enthält. |
| Unknown | `11` | Stellt den Wert einer Zelle dar, die einen #UNKNOWN!-Fehler enthält. |
| TimeOut | `19` | Stellt den Wert einer Zelle dar, die einen #TIMEOUT!-Fehler enthält. |
| External | `18` | Stellt den Wert einer Zelle dar, die einen #EXTERNAL!-Fehler enthält. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassErrorCellValueTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze eine Formel, die zu einem Spill-Fehler führt
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3;1,2,3})";
            
            try
            {
                // Berechne Formeln, um den Fehler auszulösen
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // Erwarteter Spill-Fehler
            }
            
            // Hole den erweiterten Wert der Zelle
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // Überprüfe den Fehlertyp
            if (richValue.ErrorValue == ErrorCellValueType.Spill)
            {
                Console.WriteLine("Cell contains a spill error as expected");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("ErrorCellValueTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


