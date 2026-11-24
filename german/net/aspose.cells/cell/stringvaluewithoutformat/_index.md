---
title: "Cell.StringValueWithoutFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt den Zellenwert als Zeichenkette ohne Format zurück"
type: docs
url: /de/net/aspose.cells/cell/stringvaluewithoutformat/
---
## Cell.StringValueWithoutFormat property

Gibt den Wert der Zelle als Zeichenkette ohne Format zurück.

```csharp
[Obsolete("Use GetStringValue(CellValueFormatStrategy) with CellValueFormatStrategy.None instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValueWithoutFormat { get; }
```

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Stattdessen sollte der Benutzer das Werteobjekt abrufen und es gemäß dem Werttyp und den spezifischen Anforderungen formatieren. Diese Eigenschaft wird 12 Monate später, seit Dezember 2020, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyStringValueWithoutFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie verschiedene Datentypen hinzu, um StringValueWithoutFormat zu demonstrieren
            worksheet.Cells["A1"].PutValue("Plain Text");
            worksheet.Cells["A2"].PutValue(12345);
            worksheet.Cells["A3"].PutValue(3.14159);
            worksheet.Cells["A4"].PutValue(DateTime.Now);

            // Wenden Sie Zahlenformatierung auf einige Zellen an
            Style style = worksheet.Cells["A2"].GetStyle();
            style.Number = 3; // Currency format
            worksheet.Cells["A2"].SetStyle(style);

            style = worksheet.Cells["A3"].GetStyle();
            style.Number = 9; // Percentage format
            worksheet.Cells["A3"].SetStyle(style);

            try
            {
                // Zeigen Sie StringValueWithoutFormat für jede Zelle an
                Console.WriteLine("A1 StringValueWithoutFormat: " + worksheet.Cells["A1"].StringValueWithoutFormat);
                Console.WriteLine("A2 StringValueWithoutFormat: " + worksheet.Cells["A2"].StringValueWithoutFormat);
                Console.WriteLine("A3 StringValueWithoutFormat: " + worksheet.Cells["A3"].StringValueWithoutFormat);
                Console.WriteLine("A4 StringValueWithoutFormat: " + worksheet.Cells["A4"].StringValueWithoutFormat);

                // Vergleichen Sie mit formatierter StringValue
                Console.WriteLine("\nComparison with formatted values:");
                Console.WriteLine("A2 StringValue (formatted): " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("A3 StringValue (formatted): " + worksheet.Cells["A3"].StringValue);

                // Speichere die Arbeitsmappe
                workbook.Save("StringValueWithoutFormatDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


