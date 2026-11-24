---
title: "Klasse HeaderFooterCommand"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HeaderFooterCommand Klasse. Stellt den Befehl für Kopf-/Fußzeile dar"
type: docs
url: /de/net/aspose.cells/headerfootercommand/
---
## HeaderFooterCommand class

Stellt den Befehl für Kopf-/Fußzeile dar

```csharp
public class HeaderFooterCommand
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Font](../../aspose.cells/headerfootercommand/font/) { get; } | Liefert die Schriftart des Befehlswerts. |
| [Text](../../aspose.cells/headerfootercommand/text/) { get; } | Liefert den Text des Befehls. |
| [Type](../../aspose.cells/headerfootercommand/type/) { get; } | Liefert den Typ des Kopf-/Fußzeilenbefehls. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHeaderFooterCommandDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greift auf PageSetup zu und setzt die Kopfzeile mit Befehlen
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(1, "&D&\"Arial\"sdfsdfsdfsdf");
            
            // Kopfzeilenbefehle abrufen
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(1));
            
            // Befehlstypen und Text anzeigen
            Console.WriteLine("Command 1 Type: " + commands[0].Type);
            Console.WriteLine("Command 2 Type: " + commands[1].Type);
            Console.WriteLine("Command 2 Text: " + commands[1].Text);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


