---
title: "CellsHelper.GetDateTimeFromDouble"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper method. Konvertiert den Double-Wert in den Datums‑Zeit‑Wert."
type: docs
url: /de/net/aspose.cells/cellshelper/getdatetimefromdouble/
---
## CellsHelper.GetDateTimeFromDouble method

Konvertiert den Double-Wert in einen DateTime-Wert.

```csharp
public static DateTime GetDateTimeFromDouble(double doubleValue, bool date1904)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| doubleValue | Double | Der double-Wert. |
| date1904 | Boolean | Datum-1904-System. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodGetDateTimeFromDoubleWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Daten für die Methodenparameter (Double, Boolean) vorbereiten.
            double doubleValue = 44197.5; // Represents 2021-01-01 12:00:00 in Excel serial date format
            bool date1904 = false; // Using 1900 date system

            try
            {
                // Rufen Sie die Methode GetDateTimeFromDouble mit den angegebenen Parametertypen auf.
                DateTime result = CellsHelper.GetDateTimeFromDouble(doubleValue, date1904);
                
                // Ergebnis anzeigen
                Console.WriteLine($"Converted DateTime: {result}");
                
                // Schreiben Sie das Ergebnis in eine Zelle.
                worksheet.Cells["A1"].PutValue("Original Double Value:");
                worksheet.Cells["B1"].PutValue(doubleValue);
                worksheet.Cells["A2"].PutValue("Converted DateTime:");
                worksheet.Cells["B2"].PutValue(result.ToString());
                
                Console.WriteLine("Method executed successfully with parameters (Double, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDateTimeFromDouble method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("MethodGetDateTimeFromDoubleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


