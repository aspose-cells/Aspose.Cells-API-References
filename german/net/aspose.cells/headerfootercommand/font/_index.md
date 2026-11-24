---
title: "HeaderFooterCommand.Font"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HeaderFooterCommand-Eigenschaft. Gibt die Schriftart des Befehlswertes zurück"
type: docs
url: /de/net/aspose.cells/headerfootercommand/font/
---
## HeaderFooterCommand.Font property

Liefert die Schriftart des Befehlswerts.

```csharp
public Font Font { get; }
```

### Hinweise

Unbrauchbar für HeaderFooterCommandType.Picture.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HeaderFooterCommandPropertyFontDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf die Seiteneinrichtung für Kopf-/Fußzeile
            PageSetup pageSetup = worksheet.PageSetup;

            // Setze eine Kopfzeile mit Text, die einen HeaderFooterCommand enthält
            pageSetup.SetHeader(0, "&\"Arial\"&12&BThis is a header");

            // Kopfzeilenskript abrufen
            string headerScript = pageSetup.GetHeader(0);

            // Kopfzeilenbefehle abrufen
            HeaderFooterCommand[] commands = pageSetup.GetCommands(headerScript);

            // Finde den Textbefehl (unter der Annahme, dass er der erste ist)
            if (commands.Length > 0 && commands[0].Type == HeaderFooterCommandType.Text)
            {
                HeaderFooterCommand textCommand = commands[0];
                
                // Greife auf die Font-Eigenschaft zu (schreibgeschützt)
                Font font = textCommand.Font;
                
                // Aktuelle Font-Eigenschaften anzeigen
                Console.WriteLine("Current Font:");
                Console.WriteLine($"Name: {font.Name}");
                Console.WriteLine($"Size: {font.Size}");
                Console.WriteLine($"Bold: {font.IsBold}");
                Console.WriteLine($"Color: {font.Color}");

                // Da Font schreibgeschützt ist, können wir kein neues Font-Objekt zuweisen,
                // aber wir können die Eigenschaften des bestehenden Font ändern
                font.Name = "Times New Roman";
                font.Size = 14;
                font.IsBold = false;
                font.Color = System.Drawing.Color.Blue;

                // Speichere die Arbeitsmappe, um die Änderungen zu sehen
                workbook.Save("HeaderFooterFontDemo.xlsx");

                Console.WriteLine("\nModified Font:");
                Console.WriteLine($"Name: {font.Name}");
                Console.WriteLine($"Size: {font.Size}");
                Console.WriteLine($"Bold: {font.IsBold}");
                Console.WriteLine($"Color: {font.Color}");
            }
        }
    }
}
```

### Siehe auch

* class [Font](../../font/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


