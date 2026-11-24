---
title: "AbstractTextLoadOptions.ConvertDateTimeData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractTextLoadOptions-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob die Zeichenkette in der Textdatei in Datumsdaten konvertiert wird. Der Standardwert ist true"
type: docs
url: /de/net/aspose.cells/abstracttextloadoptions/convertdatetimedata/
---
## AbstractTextLoadOptions.ConvertDateTimeData property

Liest oder setzt einen Wert, der angibt, ob die Zeichenkette in der Textdatei in Datumsdaten konvertiert wird. Standardwert ist true.

```csharp
public bool ConvertDateTimeData { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyConvertDateTimeDataDemo
    {
        public static void Run()
        {
            // Erstellen Sie CSV-Daten mit einer Datumszeichenkette
            string csvData = "\"2023-05-15\",\"123.45\"";

            // Erstellen Sie Text-Ladeoptionen, bei denen ConvertDateTimeData auf false gesetzt ist
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            options.ConvertDateTimeData = false;
            options.ConvertNumericData = false;

            // Laden Sie die CSV-Daten
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // Geben Sie die Werte aus (sollten als Zeichenketten bleiben)
            Console.WriteLine("Cell A1 value: " + worksheet.Cells[0, 0].StringValue); // Outputs "2023-05-15" as string
            Console.WriteLine("Cell B1 value: " + worksheet.Cells[0, 1].StringValue); // Outputs "123.45" as string

            // Laden Sie jetzt mit ConvertDateTimeData auf true gesetzt
            options.ConvertDateTimeData = true;
            options.ConvertNumericData = true;
            workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            worksheet = workbook.Worksheets[0];

            // Geben Sie die konvertierten Werte aus
            Console.WriteLine("Cell A1 value (converted): " + worksheet.Cells[0, 0].DateTimeValue); // Outputs DateTime
            Console.WriteLine("Cell B1 value (converted): " + worksheet.Cells[0, 1].DoubleValue);  // Outputs 123.45 as double
        }
    }
}
```

### Siehe auch

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


