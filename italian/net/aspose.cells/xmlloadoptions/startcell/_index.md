---
title: "XmlLoadOptions.StartCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlLoadOptions. Ottiene e imposta la cella di partenza"
type: docs
url: /it/net/aspose.cells/xmlloadoptions/startcell/
---
## XmlLoadOptions.StartCell property

Ottiene e imposta la cella iniziale.

```csharp
public string StartCell { get; set; }
```

### Osservazioni

Funziona solo quando il file non è speadsheetML o mappa xml su Excel.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // Crea un'istanza di XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Imposta la cella di partenza per l'importazione dei dati XML
            options.StartCell = "B2";

            // Carica un file XML in un Workbook usando le opzioni specificate
            Workbook workbook = new Workbook("input.xml", options);

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Restituisci il valore dalla cella iniziale per dimostrare la proprietà
            Console.WriteLine("Value at start cell (B2): " + worksheet.Cells["B2"].Value);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


