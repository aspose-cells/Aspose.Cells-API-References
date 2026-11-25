---
title: "XmlLoadOptions.DateFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlLoadOptions. Ottiene e imposta il formato del valore data"
type: docs
url: /it/net/aspose.cells/xmlloadoptions/dateformat/
---
## XmlLoadOptions.DateFormat property

Restituisce e imposta il formato del valore data.

```csharp
public string DateFormat { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Crea un'istanza di XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Imposta il formato della data per l'analisi delle date da XML
            options.DateFormat = "yyyy-MM-dd";
            options.ConvertNumericOrDate = true;

            // Carica un file XML in un Workbook usando le opzioni specificate
            Workbook workbook = new Workbook("input.xml", options);

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Visualizza alcune celle per dimostrare la formattazione delle date
            Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].Value);

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


