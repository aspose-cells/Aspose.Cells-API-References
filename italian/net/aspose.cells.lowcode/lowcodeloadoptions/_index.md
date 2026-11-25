---
title: "Classe LowCodeLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.LowCode.LowCodeLoadOptions. Opzioni per il caricamento del file modello"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodeloadoptions/
---
## LowCodeLoadOptions class

Opzioni per caricare il file modello.

```csharp
public class LowCodeLoadOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [LowCodeLoadOptions](lowcodeloadoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [InputFile](../../aspose.cells.lowcode/lowcodeloadoptions/inputfile/) { get; set; } | Ottiene e imposta il file (con percorso se necessario) del modello. |
| [InputStream](../../aspose.cells.lowcode/lowcodeloadoptions/inputstream/) { get; set; } | Ottiene e imposta lo Stream del modello. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            // Crea uno stream di esempio (in memoria per scopi dimostrativi)
            using (MemoryStream stream = new MemoryStream())
            {
                // Crea una nuova cartella di lavoro e salva nello stream per la demo
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Save(stream, SaveFormat.Xlsx);

                // Reimposta la posizione dello stream
                stream.Position = 0;

                // Crea e utilizza LowCodeLoadOptions
                var loadOptions = new LowCodeLoadOptions()
                {
                    InputStream = stream
                };

                // Esempio di utilizzo - verrebbe tipicamente passato a un metodo di elaborazione
                Console.WriteLine($"Loading with LowCode options from stream of length: {loadOptions.InputStream.Length}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


