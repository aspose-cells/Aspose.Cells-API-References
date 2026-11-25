---
title: "Classe LowCodeMergeOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.LowCode.LowCodeMergeOptions. Opzioni per unire più file modello in uno"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodemergeoptions/
---
## LowCodeMergeOptions class

Opzioni per unire più file modello in uno.

```csharp
public class LowCodeMergeOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [LowCodeMergeOptions](lowcodemergeoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [LoadOptionsProvider](../../aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/) { get; set; } | Provider delle opzioni di salvataggio per salvare le parti divise. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodemergeoptions/saveoptions/) { get; set; } | Opzioni di salvataggio per salvare le parti divise. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeMergeOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Crea e configura LowCodeMergeOptions
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            
            // Imposta le opzioni di salvataggio per il formato di output
            mergeOptions.SaveOptions = new LowCodeSaveOptions();
            
            // Assegna un provider personalizzato di opzioni di caricamento
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();
            
            // Esempio di integrazione (uso ipotetico con funzionalità di unione)
            // Questo verrebbe tipicamente chiamato con percorsi file reali
            // Workbook.Merge(new string[] { "template1.xlsx", "template2.xlsx" }, mergeOptions);
            
            // Salva la cartella di lavoro (scopi dimostrativi)
            workbook.Save("LowCodeMergeOptionsDemo.xlsx");
        }
    }

    // Provider personalizzato che implementa la classe astratta
    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {
        public override bool MoveNext()
        {
            // Implementazione minima per soddisfare il requisito astratto
            return false;
        }

        public override LowCodeLoadOptions Current
        {
            get { throw new InvalidOperationException(); }
        }

        public LoadOptions GetLoadOptions(string fileName)
        {
            if (fileName.EndsWith(".xlsx", StringComparison.OrdinalIgnoreCase))
            {
                return new LoadOptions(LoadFormat.Xlsx);
            }
            return new LoadOptions();
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


