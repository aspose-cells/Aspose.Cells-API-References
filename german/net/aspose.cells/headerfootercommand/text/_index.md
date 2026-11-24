---
title: "HeaderFooterCommand.Text"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HeaderFooterCommand-Eigenschaft. Gibt den Text des Befehls zurück"
type: docs
url: /de/net/aspose.cells/headerfootercommand/text/
---
## HeaderFooterCommand.Text property

Liefert den Text des Befehls.

```csharp
public string Text { get; }
```

### Hinweise

Nur gültig für HeaderFooterCommandType.Text.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze Header mit Textbefehl
            worksheet.PageSetup.SetHeader(1, "&\"Arial\"&12&KFF0000Sample Text Header");
            
            // Kopfzeilenbefehle abrufen
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(worksheet.PageSetup.GetHeader(1));
            
            // Zeige Informationen zum Textbefehl an
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
            
            // Speichere die Arbeitsmappe
            workbook.Save("HeaderFooterTextDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


