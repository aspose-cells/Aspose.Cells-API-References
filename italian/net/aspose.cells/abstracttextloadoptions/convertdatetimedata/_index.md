---
title: "AbstractTextLoadOptions.ConvertDateTimeData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AbstractTextLoadOptions. Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati di data. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/abstracttextloadoptions/convertdatetimedata/
---
## AbstractTextLoadOptions.ConvertDateTimeData property

Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati di data. Il valore predefinito è true.

```csharp
public bool ConvertDateTimeData { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyConvertDateTimeDataDemo
    {
        public static void Run()
        {
            // Crea dati CSV con una stringa di data
            string csvData = "\"2023-05-15\",\"123.45\"";

            // Crea opzioni di caricamento testo con ConvertDateTimeData impostato a false
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            options.ConvertDateTimeData = false;
            options.ConvertNumericData = false;

            // Carica i dati CSV
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // Restituisci i valori (dovrebbero rimanere come stringhe)
            Console.WriteLine("Cell A1 value: " + worksheet.Cells[0, 0].StringValue); // Outputs "2023-05-15" as string
            Console.WriteLine("Cell B1 value: " + worksheet.Cells[0, 1].StringValue); // Outputs "123.45" as string

            // Ora carica con ConvertDateTimeData impostato su true
            options.ConvertDateTimeData = true;
            options.ConvertNumericData = true;
            workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            worksheet = workbook.Worksheets[0];

            // Restituisci i valori convertiti
            Console.WriteLine("Cell A1 value (converted): " + worksheet.Cells[0, 0].DateTimeValue); // Outputs DateTime
            Console.WriteLine("Cell B1 value (converted): " + worksheet.Cells[0, 1].DoubleValue);  // Outputs 123.45 as double
        }
    }
}
```

### Vedi anche

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


