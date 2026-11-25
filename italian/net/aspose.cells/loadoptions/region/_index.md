---
title: "LoadOptions.Region"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Ottiene o imposta le impostazioni regionali utilizzate per il Workbook che verrà caricato"
type: docs
url: /it/net/aspose.cells/loadoptions/region/
---
## LoadOptions.Region property

Ottiene o imposta le impostazioni regionali utilizzate per il Workbook che verrà caricato.

```csharp
public CountryCode Region { get; set; }
```

### Osservazioni

Le impostazioni regionali possono essere utilizzate per inizializzare alcune funzionalità del workbook, come caratteri, temi e così via. Per i formati di file basati su testo, come CSV, HTML, ..., l'impostazione regionale verrà inoltre utilizzata per rilevare i formati numerici e analizzare i valori di testo in valori numerici o data/ora per le celle. Questa impostazione sarà mantenuta per il workbook istanziato in seguito, cioè, [`Region`](../../workbooksettings/region/) del workbook utilizzerà la stessa regione di questa proprietà.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyRegionDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento per il file HTML
            LoadOptions loadOpts = new LoadOptions(LoadFormat.Html);
            
            // Imposta la regione su USA
            loadOpts.Region = CountryCode.USA;
            
            // Carica il file HTML con le impostazioni regionali specificate
            Workbook wb = new Workbook("example.html", loadOpts);
            
            // Accedi al primo foglio di lavoro
            Worksheet ws = wb.Worksheets[0];
            
            // Dimostra la formattazione specifica per regione controllando lo stile di una cella
            Style style = ws.Cells["A1"].GetStyle();
            Console.WriteLine("Font used in cell A1: " + style.Font.Name);
            Console.WriteLine("Region used for loading: " + loadOpts.Region);
        }
    }
}
```

### Vedi anche

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


