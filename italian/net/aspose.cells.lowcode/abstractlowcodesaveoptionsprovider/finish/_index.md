---
title: "AbstractLowCodeSaveOptionsProvider.Finish"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractLowCodeSaveOptionsProvider. Rilascia le risorse dopo l'elaborazione della parte attualmente suddivisa"
type: docs
url: /it/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/
---
## AbstractLowCodeSaveOptionsProvider.Finish method

Rilascia le risorse dopo l'elaborazione della parte attualmente divisa.

```csharp
public virtual void Finish(LowCodeSaveOptions part)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| parte | LowCodeSaveOptions | le opzioni di salvataggio utilizzate per la parte attualmente suddivisa. |

### Osservazioni

Per impostazione predefinita questo metodo chiude semplicemente lo stream specificato da [`OutputStream`](../../lowcodesaveoptions/outputstream/) direttamente (se le opzioni di salvataggio hanno specificato uno Stream come destinazione). L'utente può sovrascrivere questo metodo per controllare come rilasciare le risorse in base alle proprie esigenze e all'implementazione di [`GetSaveOptions`](../getsaveoptions/).

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo
    {
        public static void Run()
        {

            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "split.xlsx";

            // Crea un'istanza concreta del provider
            var provider = new CustomLowCodeSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
                     
          
        }
    }

    // Implementazione concreta di AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        { 
            base.Finish(part);
        }
        // Implementa il metodo astratto richiesto
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


