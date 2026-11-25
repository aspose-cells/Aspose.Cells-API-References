---
title: "HeaderFooterCommand.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HeaderFooterCommand. Ottiene il tipo di comando intestazione/piè di pagina"
type: docs
url: /it/net/aspose.cells/headerfootercommand/type/
---
## HeaderFooterCommand.Type property

Ottiene il tipo di comando intestazione/piè di pagina.

```csharp
public HeaderFooterCommandType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HeaderFooterCommandPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta l'intestazione con diversi tipi di comando
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(0, "&D&\"Arial\"&12sdfsdfsdfsdf");
            
            // Ottieni i comandi di intestazione
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(0));
            
            // Dimostra l'uso della proprietà Type
            Console.WriteLine("Command 0 Type: " + commands[0].Type); // CurrentDate
            Console.WriteLine("Command 1 Type: " + commands[1].Type); // Text
            Console.WriteLine("Command 1 Text: " + commands[1].Text); // sdfsdfsdfsdf
        }
    }
}
```

### Vedi anche

* enum [HeaderFooterCommandType](../../headerfootercommandtype/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


