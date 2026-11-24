---
title: "Enum HeaderFooterCommandType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HeaderFooterCommandType-Enum. Stellt den Befehlstyp von Kopf- und Fußzeile dar"
type: docs
url: /de/net/aspose.cells/headerfootercommandtype/
---
## HeaderFooterCommandType enumeration

Stellt den Befehlstyp von Kopf‑ und Fußzeile dar.

```csharp
public enum HeaderFooterCommandType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Text | `0` | Der Text. |
| CurrentPage | `1` | Aktuelle Seitenzahl |
| Pagecount | `2` | Seitenanzahl |
| CurrentDate | `3` | Aktuelles Datum |
| CurrentTime | `4` | Aktuelle Uhrzeit |
| SheetName | `5` | Blattname |
| FileName | `6` | Dateiname ohne Pfad |
| FilePath | `7` | Dateipfad ohne Dateiname |
| Picture | `8` | Bild |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHeaderFooterCommandTypeDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Kopfzeile mit verschiedenen Befehlsarten festlegen
                worksheet.PageSetup.SetHeader(0, "&[Page] of &[Pages] - &[Date] - &[Time] - &[File]");

                // Kopfzeilenbefehle abrufen
                string headerScript = worksheet.PageSetup.GetHeader(0);
                HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(headerScript);

                // Verschiedene Werte von HeaderFooterCommandType demonstrieren
                foreach (HeaderFooterCommand cmd in commands)
                {
                    Console.WriteLine($"Command Type: {cmd.Type}");

                    // Auf bestimmte Befehlsarten prüfen
                    if (cmd.Type == HeaderFooterCommandType.CurrentPage)
                    {
                        Console.WriteLine("Found CurrentPage command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.Pagecount)
                    {
                        Console.WriteLine("Found Pagecount command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.CurrentDate)
                    {
                        Console.WriteLine("Found CurrentDate command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.CurrentTime)
                    {
                        Console.WriteLine("Found CurrentTime command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.FileName)
                    {
                        Console.WriteLine("Found FileName command");
                    }
                }

                // Arbeitsmappe speichern, um die Kopfzeilenkonfiguration zu demonstrieren
                workbook.Save("HeaderFooterCommandTypeDemo.xlsx");
                Console.WriteLine("HeaderFooterCommandType demonstration completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HeaderFooterCommandType: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


