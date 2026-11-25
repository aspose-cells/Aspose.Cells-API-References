---
title: "AbstractTextLoadOptions.ConvertNumericData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AbstractTextLoadOptions. Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati numerici. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/abstracttextloadoptions/convertnumericdata/
---
## AbstractTextLoadOptions.ConvertNumericData property

Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati numerici. Il valore predefinito è true.

```csharp
public bool ConvertNumericData { get; set; }
```

### Esempi

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
            // Crea dati CSV di esempio con valori numerici e stringhe
            string csvData = "ID,Name,Price,Quantity\n" +
                            "1,Product A,19.99,5\n" +
                            "2,Product B,\"24.50\",\"10\"\n" +
                            "3,Product C,15.75,\"N/A\"";

            // Crea TxtLoadOptions con ConvertNumericData impostato su true
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv)
            {
                ConvertNumericData = true,
                ConvertDateTimeData = true
            };

            // Carica i dati CSV in una cartella di lavoro
            Workbook workbook = new Workbook(new System.IO.MemoryStream(Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // Dimostra la conversione numerica
            Console.WriteLine("Cell B2 (Product A Price) value type: " + worksheet.Cells["B2"].Value.GetType());
            Console.WriteLine("Cell B2 value: " + worksheet.Cells["B2"].Value);

            // Dimostra i valori stringa che non possono essere convertiti
            Console.WriteLine("\nCell D4 (N/A) value type: " + worksheet.Cells["D4"].Value.GetType());
            Console.WriteLine("Cell D4 value: " + worksheet.Cells["D4"].Value);

            // Mostra come i numeri tra virgolette vengano comunque convertiti quando ConvertNumericData è true
            Console.WriteLine("\nCell C3 (Quoted \"24.50\") value type: " + worksheet.Cells["C3"].Value.GetType());
            Console.WriteLine("Cell C3 value: " + worksheet.Cells["C3"].Value);
        }
    }
}
```

### Vedi anche

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


