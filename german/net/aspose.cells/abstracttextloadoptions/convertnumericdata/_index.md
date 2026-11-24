---
title: "AbstractTextLoadOptions.ConvertNumericData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractTextLoadOptions-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird. Der Standardwert ist true"
type: docs
url: /de/net/aspose.cells/abstracttextloadoptions/convertnumericdata/
---
## AbstractTextLoadOptions.ConvertNumericData property

Liest oder setzt einen Wert, der angibt, ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird. Standardwert ist true.

```csharp
public bool ConvertNumericData { get; set; }
```

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Erstelle Beispieldaten im CSV-Format mit numerischen und Zeichenkettenwerten
            string csvData = "ID,Name,Price,Quantity\n" +
                            "1,Product A,19.99,5\n" +
                            "2,Product B,\"24.50\",\"10\"\n" +
                            "3,Product C,15.75,\"N/A\"";

            // Erstelle TxtLoadOptions mit ConvertNumericData auf true gesetzt
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv)
            {
                ConvertNumericData = true,
                ConvertDateTimeData = true
            };

            // Lade die CSV-Daten in eine Arbeitsmappe
            Workbook workbook = new Workbook(new System.IO.MemoryStream(Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstriere numerische Konvertierung
            Console.WriteLine("Cell B2 (Product A Price) value type: " + worksheet.Cells["B2"].Value.GetType());
            Console.WriteLine("Cell B2 value: " + worksheet.Cells["B2"].Value);

            // Demonstriere Zeichenkettenwerte, die nicht konvertiert werden konnten
            Console.WriteLine("\nCell D4 (N/A) value type: " + worksheet.Cells["D4"].Value.GetType());
            Console.WriteLine("Cell D4 value: " + worksheet.Cells["D4"].Value);

            // Zeige, wie zitierte Zahlen weiterhin konvertiert werden, wenn ConvertNumericData auf true gesetzt ist
            Console.WriteLine("\nCell C3 (Quoted \"24.50\") value type: " + worksheet.Cells["C3"].Value.GetType());
            Console.WriteLine("Cell C3 value: " + worksheet.Cells["C3"].Value);
        }
    }
}
```

### Siehe auch

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


