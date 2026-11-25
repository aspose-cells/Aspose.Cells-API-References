---
title: "HeaderFooterCommand.Text"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HeaderFooterCommand. Ottiene il testo del comando"
type: docs
url: /it/net/aspose.cells/headerfootercommand/text/
---
## HeaderFooterCommand.Text property

Ottiene il testo del comando.

```csharp
public string Text { get; }
```

### Osservazioni

Valido solo per HeaderFooterCommandType.Text.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class HeaderFooterCommandPropertyTextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta l'intestazione con il comando di testo
            worksheet.PageSetup.SetHeader(1, "&\"Arial\"&12&KFF0000Sample Text Header");
            
            // Ottieni i comandi di intestazione
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(worksheet.PageSetup.GetHeader(1));
            
            // Visualizza le informazioni sul comando di testo
            foreach (HeaderFooterCommand cmd in commands)
            {
                if (cmd.Type == HeaderFooterCommandType.Text)
                {
                    Console.WriteLine("Text command found:");
                    Console.WriteLine("Text: " + cmd.Text);
                    Console.WriteLine("Font: " + cmd.Font);
                    Console.WriteLine("Color: " + ColorTranslator.ToHtml(cmd.Font.Color));
                }
            }
            
            // Salva la cartella di lavoro
            workbook.Save("HeaderFooterTextDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


