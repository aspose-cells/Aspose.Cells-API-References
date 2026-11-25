---
title: "Classe LowCodeSplitOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.LowCode.LowCodeSplitOptions. Opzioni per la divisione del foglio di calcolo"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesplitoptions/
---
## LowCodeSplitOptions class

Opzioni per dividere il foglio di calcolo.

```csharp
public class LowCodeSplitOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [LowCodeSplitOptions](lowcodesplitoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [LoadOptions](../../aspose.cells.lowcode/lowcodesplitoptions/loadoptions/) { get; set; } | Opzioni di caricamento per il foglio di calcolo che verrà diviso. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptions/) { get; set; } | Opzioni di salvataggio per salvare le parti divise. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/) { get; set; } | Provider delle opzioni di salvataggio per salvare le parti divise. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeSplitOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola il foglio di lavoro con dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Data for Splitting");
            
            // Crea un'istanza di LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // Configura LoadOptions (esempio: gestisci una sorgente protetta da password)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // Configura SaveOptions (esempio: imposta il formato di output predefinito)
            splitOptions.SaveOptions = new LowCodeSaveOptions();
            
            // Implementa un provider personalizzato di SaveOptions per impostazioni di output dinamiche
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // Esempio di integrazione: dividi la cartella di lavoro in parti usando le opzioni configurate
            // (Supponi l'esistenza di un metodo come LowCodeEngine.Split(workbook, splitOptions, "outputDir"))
            // LowCodeEngine.Split(workbook, splitOptions, "OutputDirectory");
            
            // Salva la cartella di lavoro originale per la dimostrazione
            workbook.Save("LowCodeSplitOptionsDemo.xlsx");
        }

        // Implementazione personalizzata di SaveOptionsProvider
        private class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
        {
            public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
            {
                // Logica di esempio: impostazioni alternate in base all'indice di divisione
                return new LowCodeSaveOptions();
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


