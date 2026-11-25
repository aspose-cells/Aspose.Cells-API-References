---
title: "LowCodeSplitOptions.SaveOptionsProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSplitOptions. Fornitore delle opzioni di salvataggio per salvare le parti suddivise"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/
---
## LowCodeSplitOptions.SaveOptionsProvider property

Provider delle opzioni di salvataggio per salvare le parti divise.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### Osservazioni

Se questa proprietà è specificata, [`SaveOptions`](../saveoptions/) non ha alcun effetto perché l'output di ogni parte suddivisa sarà specificato dal fornitore.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // Crea un'istanza di LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // Mostra il valore corrente di SaveOptionsProvider (null per impostazione predefinita)
            Console.WriteLine("Current SaveOptionsProvider value: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // Crea un SaveOptionsProvider personalizzato
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // Dimostra l'effetto dell'impostazione di SaveOptionsProvider
            // In uno scenario reale, questo verrebbe utilizzato durante la suddivisione dei file
            Console.WriteLine("After setting SaveOptionsProvider: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // Salva la cartella di lavoro (anche se la suddivisione non è dimostrata qui)
            workbook.Save("PropertySaveOptionsProviderDemo.xlsx");
        }
    }

    // Implementazione personalizzata di AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Crea opzioni di salvataggio personalizzate per ogni parte suddivisa
            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            return options;
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Esegui eventuali operazioni di pulizia dopo aver salvato ogni parte
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### Vedi anche

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


