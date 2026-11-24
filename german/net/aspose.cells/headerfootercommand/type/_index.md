---
title: "HeaderFooterCommand.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HeaderFooterCommand-Eigenschaft. Gibt den Header/Footer-Befehlstyp zurück"
type: docs
url: /de/net/aspose.cells/headerfootercommand/type/
---
## HeaderFooterCommand.Type property

Liefert den Typ des Kopf-/Fußzeilenbefehls.

```csharp
public HeaderFooterCommandType Type { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HeaderFooterCommandPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Kopfzeile mit verschiedenen Befehlsarten festlegen
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(0, "&D&\"Arial\"&12sdfsdfsdfsdf");
            
            // Kopfzeilenbefehle abrufen
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(0));
            
            // Demonstriere die Verwendung der Type‑Eigenschaft
            Console.WriteLine("Command 0 Type: " + commands[0].Type); // CurrentDate
            Console.WriteLine("Command 1 Type: " + commands[1].Type); // Text
            Console.WriteLine("Command 1 Text: " + commands[1].Text); // sdfsdfsdfsdf
        }
    }
}
```

### Siehe auch

* enum [HeaderFooterCommandType](../../headerfootercommandtype/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


