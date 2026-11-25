---
title: "Classe LoadFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.LoadFilter. Rappresenta il filtro che fornisce opzioni per il caricamento dei dati quando si carica una cartella di lavoro da un modello"
type: docs
url: /it/net/aspose.cells/loadfilter/
---
## LoadFilter class

Rappresenta il filtro che fornisce opzioni per il caricamento dei dati quando si carica la cartella di lavoro da un modello.

```csharp
public class LoadFilter
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [LoadFilter](loadfilter/#constructor)() | Crea un LoadFilter con le opzioni di filtro predefinite LoadDataFilterOptions.All. |
| [LoadFilter](loadfilter/#constructor_1)(LoadDataFilterOptions) | Crea un LoadFilter con le opzioni di filtro specificate. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [LoadDataFilterOptions](../../aspose.cells/loadfilter/loaddatafilteroptions/) { get; set; } | Le opzioni di filtro per indicare quali dati devono essere caricati. |
| virtual [SheetsInLoadingOrder](../../aspose.cells/loadfilter/sheetsinloadingorder/) { get; } | Specifica i fogli (indici) e l'ordine da caricare. Il valore predefinito è null, il che indica di caricare tutti i fogli nell'ordine predefinito nel file modello. Se non è null e l'indice di qualche foglio non è presente nell'array restituito, allora il foglio non verrà caricato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [StartSheet](../../aspose.cells/loadfilter/startsheet/)(Worksheet) | Prepara le opzioni di filtro prima di caricare il foglio di lavoro specificato. L'implementazione dell'utente di LoadFilter può modificare le LoadDataFilterOptions qui per indicare come caricare i dati per questo foglio di lavoro. |

### Osservazioni

L'utente può specificare le opzioni di filtro o implementare il proprio LoadFilter per indicare come caricare i dati.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterDemo
    {
        public static void LoadFilterExample()
        {
            // Crea LoadOptions e imposta LoadFilter
            LoadOptions opts = new LoadOptions();
            opts.LoadFilter = new CustomLoadFilter();

            // Carica la cartella di lavoro con le LoadOptions specificate
            Workbook wb = new Workbook("LoadFilterExample_original.xlsx", opts);

            // Salva la cartella di lavoro per vedere l'effetto di LoadFilter
            wb.Save("LoadFilterExample.xlsx");
        }

        // Implementazione personalizzata di LoadFilter
        public class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                if (sheet.Name == "Sheet1")
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.All;
                }
                else
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.Structure;
                }
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


