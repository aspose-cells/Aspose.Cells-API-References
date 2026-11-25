---
title: "XmlLoadOptions.NumberFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlLoadOptions. Ottiene e imposta il formato del valore numerico"
type: docs
url: /it/net/aspose.cells/xmlloadoptions/numberformat/
---
## XmlLoadOptions.NumberFormat property

Ottiene e imposta il formato del valore numerico.

```csharp
public string NumberFormat { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Crea un'istanza di XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Imposta la proprietà NumberFormat per visualizzare i numeri con 2 cifre decimali
            options.NumberFormat = "0.00";

            // Carica un file XML in un Workbook usando le opzioni specificate
            Workbook workbook = new Workbook("input.xml", options);

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta alcuni valori numerici per dimostrare la formattazione dei numeri
            worksheet.Cells["A1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(45.678);
            worksheet.Cells["A3"].PutValue(0.5);

            // Salva la cartella di lavoro in un nuovo file
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


