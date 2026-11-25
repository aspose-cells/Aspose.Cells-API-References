---
title: "LoadFilter.SheetsInLoadingOrder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadFilter. Specifica gli indici dei fogli e l'ordine da caricare. Il valore predefinito è null, che indica di caricare tutti i fogli nell'ordine predefinito nel file modello. Se non è null e qualche indice di foglio non è presente nell'array restituito, allora il foglio non verrà caricato"
type: docs
url: /it/net/aspose.cells/loadfilter/sheetsinloadingorder/
---
## LoadFilter.SheetsInLoadingOrder property

Specifica i fogli (indici) e l'ordine da caricare. Il valore predefinito è null, il che indica di caricare tutti i fogli nell'ordine predefinito nel file modello. Se non è null e l'indice di qualche foglio non è presente nell'array restituito, allora il foglio non verrà caricato.

```csharp
public virtual int[] SheetsInLoadingOrder { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterPropertySheetsInLoadingOrderDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con più fogli
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Crea un filtro di caricamento personalizzato
            LoadFilter loadFilter = new LoadFilter(LoadDataFilterOptions.All);
            
            // Visualizza il valore predefinito di SheetsInLoadingOrder (null significa caricare tutti i fogli)
            Console.WriteLine("Initial SheetsInLoadingOrder is null: " + (loadFilter.SheetsInLoadingOrder == null));
            
            // Crea un file modello per dimostrare il caricamento con ordine dei fogli personalizzato
            workbook.Save("Template.xlsx");
            
            // Crea le opzioni di caricamento con il nostro filtro personalizzato
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = loadFilter;
            
            // Carica la cartella di lavoro con le impostazioni predefinite (tutti i fogli)
            Workbook loadedWorkbook1 = new Workbook("Template.xlsx", loadOptions);
            Console.WriteLine("Sheets loaded with default filter: " + loadedWorkbook1.Worksheets.Count);
            
            // Crea un nuovo filtro con un ordine di caricamento dei fogli specifico
            LoadFilter orderedFilter = new LoadFilter(LoadDataFilterOptions.All)
            {
                // Nota: SheetsInLoadingOrder è di sola lettura, quindi dobbiamo creare un nuovo filtro
                // con l'ordine desiderato nel costruttore o tramite altri metodi
                // Questo dimostra la limitazione della proprietà di essere di sola lettura
            };
            
            // Poiché SheetsInLoadingOrder è di sola lettura, dovremo creare una sottoclasse di LoadFilter
            // per dimostrare l'ordine di caricamento dei fogli personalizzato
            CustomLoadFilter customFilter = new CustomLoadFilter(new int[] { 2, 0 }); // Load Sheet3 first, then Sheet1
            
            LoadOptions customLoadOptions = new LoadOptions();
            customLoadOptions.LoadFilter = customFilter;
            
            // Carica la cartella di lavoro con ordine dei fogli personalizzato
            Workbook loadedWorkbook2 = new Workbook("Template.xlsx", customLoadOptions);
            Console.WriteLine("Sheets loaded with custom filter: " + loadedWorkbook2.Worksheets.Count);
            Console.WriteLine("First sheet in custom order: " + loadedWorkbook2.Worksheets[0].Name);
        }
    }

    // Implementazione personalizzata di LoadFilter per dimostrare la funzionalità di SheetsInLoadingOrder
    public class CustomLoadFilter : LoadFilter
    {
        private readonly int[] _sheetsOrder;
        
        public CustomLoadFilter(int[] sheetsOrder) : base(LoadDataFilterOptions.All)
        {
            _sheetsOrder = sheetsOrder;
        }
        
        public override int[] SheetsInLoadingOrder => _sheetsOrder;
    }
}
```

### Vedi anche

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


