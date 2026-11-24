---
title: "UnionRange.PutValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Methode. Fügt einen Wert in den Bereich ein; falls zutreffend wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zellen wird zurückgesetzt"
type: docs
url: /de/net/aspose.cells/unionrange/putvalue/
---
## UnionRange.PutValue method

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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen Union-Bereich, der die Zellen A1 bis B2 abdeckt
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
            
            try
            {
                // Rufe PutValue mit den Parametern auf: (String, Boolean, Boolean)
                unionRange.PutValue("Sample Value", true, true);
                
                Console.WriteLine("PutValue method executed successfully with parameters (String, Boolean, Boolean)");
                
                // Zeige die Bereichsinformationen an, um die Wirkung zu zeigen
                Console.WriteLine($"Range address: {unionRange.RefersTo}");
                Console.WriteLine($"Value set in range: {unionRange.Value}");
                
                // Wende Formatierungen an, um die Wirkung sichtbar zu machen
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                style.HorizontalAlignment = TextAlignmentType.Center;
                unionRange.SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PutValue method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("UnionRangeMethodPutValueWithStringBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


