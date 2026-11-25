---
title: "AbstractLowCodeLoadOptionsProvider.Finish"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractLowCodeLoadOptionsProvider. Rilascia le risorse dopo aver elaborato la parte corrente dell'input"
type: docs
url: /it/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/
---
## AbstractLowCodeLoadOptionsProvider.Finish method

Rilascia le risorse dopo aver elaborato la parte corrente dell'input.

```csharp
public virtual void Finish(LowCodeLoadOptions part)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| parte | LowCodeLoadOptions | le opzioni di caricamento usate per la parte attualmente divisa. |

### Osservazioni

Per impostazione predefinita questo metodo chiude semplicemente lo stream specificato da [`InputStream`](../../lowcodeloadoptions/inputstream/) direttamente (se le opzioni di caricamento hanno specificato uno Stream come origine). L'utente può sovrascrivere questo metodo per controllare come rilasciare le risorse in base alle proprie esigenze e all'implementazione di [`Current`](../current/).

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.Collections;

    public class AbstractLowCodeLoadOptionsProviderMethodFinishWithLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };

            CustomLoadOptionsProvider provider = new CustomLoadOptionsProvider(files);

            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.OutputFile = "result.xlsx";
            saveOptions.SaveFormat = SaveFormat.Xlsx;

            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            mergeOptions.LoadOptionsProvider = provider;
            mergeOptions.SaveOptions = saveOptions;

            SpreadsheetMerger.Process(mergeOptions);
        }
    }

    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {       

        public IEnumerator fileIter;
        public CustomLoadOptionsProvider(string[] files)
        {
            fileIter = files.GetEnumerator();
            current = new LowCodeLoadOptions();
        }
        private LowCodeLoadOptions current;

        public override LowCodeLoadOptions Current => current;

        public override bool MoveNext()
        {
            if (fileIter.MoveNext())
            {
                current = new LowCodeLoadOptions();
                current.InputFile = fileIter.Current.ToString();
                return true;
            }
            
            return false;
        }

        public override void Finish(LowCodeLoadOptions part)
        {
            base.Finish(part);
        }
    }
}
```

### Vedi anche

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


