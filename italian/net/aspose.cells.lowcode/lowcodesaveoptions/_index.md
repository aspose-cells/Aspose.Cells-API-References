---
title: "Classe LowCodeSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.LowCode.LowCodeSaveOptions. Opzioni per salvare i risultati generati in modalità low‑code"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptions/
---
## LowCodeSaveOptions class

Opzioni per salvare i risultati generati in modalità low code.

```csharp
public class LowCodeSaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [LowCodeSaveOptions](lowcodesaveoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Ottiene e imposta il file (con percorso se necessario) per salvare i dati generati. Quando si imposta questa proprietà con un valore diverso da null o stringa vuota, [`OutputStream`](./outputstream/) verrà ignorato. |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Ottiene e imposta lo Stream per scrivere i dati generati. Quando si imposta questa proprietà con un valore diverso da null, [`OutputFile`](./outputfile/) verrà ignorato. |
| virtual [SaveFormat](../../aspose.cells.lowcode/lowcodesaveoptions/saveformat/) { get; set; } | Ottiene e imposta il formato di salvataggio per l'output. In generale, per processi specifici in modalità low‑code, sono consentiti solo alcuni formati specifici. Si prega di specificare il formato corretto per il processo corrispondente, altrimenti potrebbero verificarsi risultati inattesi o addirittura eccezioni. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeSaveOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e inserisci alcuni dati
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Crea opzioni di salvataggio
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions()
            {
                OutputFile = "output.xlsx"
            };

            // Salva la cartella di lavoro usando le opzioni specificate
            workbook.Save(saveOptions.OutputFile, saveOptions.SaveFormat);
            
            Console.WriteLine("File saved successfully with LowCodeSaveOptions");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


