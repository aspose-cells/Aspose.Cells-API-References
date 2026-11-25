---
title: "FindOptions.ConvertNumericData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FindOptions. Ottiene o imposta un valore che indica se convertire il valore della stringa cercata in dati numerici"
type: docs
url: /it/net/aspose.cells/findoptions/convertnumericdata/
---
## FindOptions.ConvertNumericData property

Ottiene o imposta un valore che indica se convertire il valore della stringa cercata in dati numerici.

```csharp
public bool ConvertNumericData { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio includendo valori numerici come stringhe
            worksheet.Cells["A1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("456");
            worksheet.Cells["A3"].PutValue("01/28/2010");

            // Crea le opzioni di ricerca e imposta ConvertNumericData su true
            FindOptions options = new FindOptions();
            options.ConvertNumericData = true;

            // Trova il valore della data (memorizzato come stringa ma convertito in numerico durante la ricerca)
            Cell foundCell = worksheet.Cells.Find("01/28/2010", null, options);

            // Restituisci il risultato
            if (foundCell != null)
            {
                Console.WriteLine("Found value at: " + foundCell.Name);
                Console.WriteLine("Cell value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("Value not found");
            }
        }
    }
}
```

### Vedi anche

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


