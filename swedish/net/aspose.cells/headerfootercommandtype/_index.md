---
title: "Enum HeaderFooterCommandType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HeaderFooterCommandType enum. Representerar kommandotypen för sidhuvud och sidfot"
type: docs
url: /sv/net/aspose.cells/headerfootercommandtype/
---
## HeaderFooterCommandType enumeration

Representerar kommandotypen för sidhuvud och sidfot.

```csharp
public enum HeaderFooterCommandType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Text | `0` | Texten. |
| CurrentPage | `1` | Aktuellt sidnummer |
| Pagecount | `2` | Sidantal |
| CurrentDate | `3` | Aktuellt datum |
| CurrentTime | `4` | Aktuell tid |
| SheetName | `5` | Bladnamn |
| FileName | `6` | Filnamn utan sökväg |
| FilePath | `7` | Sökväg utan filnamn |
| Picture | `8` | Bild |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHeaderFooterCommandTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ställ in sidhuvud med olika kommandotyper
                worksheet.PageSetup.SetHeader(0, "&[Page] of &[Pages] - &[Date] - &[Time] - &[File]");

                // Hämta sidhuvudskommandon
                string headerScript = worksheet.PageSetup.GetHeader(0);
                HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(headerScript);

                // Demonstrera olika HeaderFooterCommandType‑värden
                foreach (HeaderFooterCommand cmd in commands)
                {
                    Console.WriteLine($"Command Type: {cmd.Type}");

                    // Kontrollera specifika kommandotyper
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

                // Spara arbetsboken för att demonstrera sidhuvudskonfiguration
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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


