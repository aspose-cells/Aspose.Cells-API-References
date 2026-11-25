---
title: "PageSetup.GetCommands"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Ottiene tutti i comandi dell'intestazione o del piè di pagina"
type: docs
url: /it/net/aspose.cells/pagesetup/getcommands/
---
## PageSetup.GetCommands method

Ottiene tutti i comandi di intestazione o piè di pagina.

```csharp
public HeaderFooterCommand[] GetCommands(string headerFooterScript)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| headerFooterScript | String | Lo script dell'intestazione/piè di pagina |

### Valore di ritorno

Restituisce tutti i comandi dell'intestazione o del piè di pagina.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetCommandsWithStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta l'intestazione con i comandi
            string header = "&D&\"Arial\"&12sdfsdfsdfsdf";
            worksheet.PageSetup.SetHeader(1, header);
            
            // Ottieni i comandi di intestazione
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(header);
            
            // Visualizza i tipi di comando e il testo
            foreach (HeaderFooterCommand cmd in commands)
            {
                Console.WriteLine($"Type: {cmd.Type}, Text: {cmd.Text}");
            }
        }
    }
}
```

### Vedi anche

* class [HeaderFooterCommand](../../headerfootercommand/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


