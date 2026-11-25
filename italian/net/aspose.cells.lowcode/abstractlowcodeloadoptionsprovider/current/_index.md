---
title: "AbstractLowCodeLoadOptionsProvider.Current"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AbstractLowCodeLoadOptionsProvider. Ottiene le opzioni di caricamento da cui caricare i dati della parte attualmente elaborata"
type: docs
url: /it/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/
---
## AbstractLowCodeLoadOptionsProvider.Current property

Ottiene le opzioni di caricamento da cui caricare i dati della parte attualmente elaborata.

```csharp
public abstract LowCodeLoadOptions Current { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.Collections;

    public class AbstractLowCodeLoadOptionsProviderPropertyCurrentDemo
    {
        public static void Run()
        {
            string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };
            // Inizializza il provider personalizzato con le nostre opzioni di caricamento
            CustomProvider provider = new CustomProvider(files);
            
            int counter = 1;
            while (provider.MoveNext())
            {
                // Accedi alla proprietà Current per ottenere le opzioni di caricamento attive
                Console.WriteLine($"Processing set {counter}");
                    
                // Crea una cartella di lavoro usando il file/stream di input delle attuali opzioni di caricamento
                Workbook workbook;
                if (provider.Current.InputFile != null)
                {
                    workbook = new Workbook(provider.Current.InputFile);
                }
                else if (provider.Current.InputStream != null)
                {
                    workbook = new Workbook(provider.Current.InputStream);
                }
                else
                {
                    workbook = new Workbook();
                }

                Worksheet worksheet = workbook.Worksheets[0];

                // Dimostra l'impatto dell'opzione rimosso a causa della proprietà mancante
                worksheet.Cells["A1"].Value = "Sample Value";

                // Salva il risultato
                workbook.Save($"CurrentDemo_{counter}.xlsx");
                counter++;
            }
        }
    }

    // Implementazione di provider personalizzato con IDisposable
    public class CustomProvider : AbstractLowCodeLoadOptionsProvider
    {
        
        public IEnumerator fileIter;

        public CustomProvider(string[] files)
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


