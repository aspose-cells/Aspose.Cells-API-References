---
title: "PageSetup.GetCommands"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup‑Methode. Gibt alle Befehle von Kopf‑ oder Fußzeile zurück"
type: docs
url: /de/net/aspose.cells/pagesetup/getcommands/
---
## PageSetup.GetCommands method

Ruft alle Befehle der Kopf- oder Fußzeile ab.

```csharp
public HeaderFooterCommand[] GetCommands(string headerFooterScript)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| headerFooterScript | String | Das header/footer‑Skript |

### Rückgabewert

Gibt alle Befehle von Kopf‑ oder Fußzeile zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetCommandsWithStringDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Kopfzeile mit Befehlen festlegen
            string header = "&D&\"Arial\"&12sdfsdfsdfsdf";
            worksheet.PageSetup.SetHeader(1, header);
            
            // Kopfzeilenbefehle abrufen
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(header);
            
            // Befehlstypen und Text anzeigen
            foreach (HeaderFooterCommand cmd in commands)
            {
                Console.WriteLine($"Type: {cmd.Type}, Text: {cmd.Text}");
            }
        }
    }
}
```

### Siehe auch

* class [HeaderFooterCommand](../../headerfootercommand/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


