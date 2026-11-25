---
title: "LowCodeMergeOptions.LoadOptionsProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "LowCodeMergeOptions proprietà. Provider delle opzioni di salvataggio per salvare le parti divise"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/
---
## LowCodeMergeOptions.LoadOptionsProvider property

Provider delle opzioni di salvataggio per salvare le parti divise.

```csharp
public AbstractLowCodeLoadOptionsProvider LoadOptionsProvider { get; set; }
```

### Osservazioni

Se questa proprietà è specificata, [`LoadOptions`](../../../aspose.cells/loadoptions/) non ha effetto perché l'output di ogni parte divisa sarà specificato dal provider.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeMergeOptionsPropertyLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di LowCodeMergeOptions
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();

            // Visualizza il valore corrente di LoadOptionsProvider (dovrebbe essere null inizialmente)
            Console.WriteLine("Current LoadOptionsProvider value: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // Crea un'implementazione personalizzata di LoadOptionsProvider
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();

            // Dimostra l'impostazione della proprietà
            Console.WriteLine("After setting LoadOptionsProvider: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // Usa le opzioni di merge con il provider
            // Questo verrebbe tipicamente usato con metodi che elaborano più file
            // Per dimostrazione, controlleremo solo se il provider può passare al successivo
            bool hasNext = mergeOptions.LoadOptionsProvider.MoveNext();
            Console.WriteLine("LoadOptionsProvider MoveNext result: " + hasNext);

            // Salva la cartella di lavoro
            workbook.Save("PropertyLoadOptionsProviderDemo.xlsx");
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int counter = 0;
            private readonly LowCodeLoadOptions options = new LowCodeLoadOptions();

            public override LowCodeLoadOptions Current => options;

            public override bool MoveNext()
            {
                // Simula la presenza di 3 file da elaborare
                if (counter < 3)
                {
                    counter++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // La logica di pulizia o finalizzazione andrebbe qui
            }
        }
    }
}
```

### Vedi anche

* class [AbstractLowCodeLoadOptionsProvider](../../abstractlowcodeloadoptionsprovider/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


