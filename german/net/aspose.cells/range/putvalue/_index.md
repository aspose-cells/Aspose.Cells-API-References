---
title: "Range.PutValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Fügt einen Wert in den Range ein; falls zutreffend wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zellen wird zurückgesetzt."
type: docs
url: /de/net/aspose.cells/range/putvalue/
---
## Range.PutValue method

Setzt einen Wert in den Bereich; falls zutreffend wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringValue | String | Eingabewert |
| isConverted | Boolean | True: in einen anderen Datentyp konvertiert, falls zutreffend. |
| setStyle | Boolean | True: das Zahlenformat auf den Zellenstil setzen, wenn in einen anderen Datentyp konvertiert wird |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1:B10");
            range.PutValue("123", true, false);
            
            Console.WriteLine("Value at A5: " + cells["A5"].DoubleValue);
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


