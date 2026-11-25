---
title: "Classe HeaderFooterCommand"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.HeaderFooterCommand. Rappresenta il comando di intestazione/piè di pagina"
type: docs
url: /it/net/aspose.cells/headerfootercommand/
---
## HeaderFooterCommand class

Rappresenta il comando di intestazione/piè di pagina

```csharp
public class HeaderFooterCommand
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Font](../../aspose.cells/headerfootercommand/font/) { get; } | Ottiene il carattere del valore del comando. |
| [Text](../../aspose.cells/headerfootercommand/text/) { get; } | Ottiene il testo del comando. |
| [Type](../../aspose.cells/headerfootercommand/type/) { get; } | Ottiene il tipo di comando intestazione/piè di pagina. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHeaderFooterCommandDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi a PageSetup e imposta l'intestazione con i comandi
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(1, "&D&\"Arial\"sdfsdfsdfsdf");
            
            // Ottieni i comandi di intestazione
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(1));
            
            // Visualizza i tipi di comando e il testo
            Console.WriteLine("Command 1 Type: " + commands[0].Type);
            Console.WriteLine("Command 2 Type: " + commands[1].Type);
            Console.WriteLine("Command 2 Text: " + commands[1].Text);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


