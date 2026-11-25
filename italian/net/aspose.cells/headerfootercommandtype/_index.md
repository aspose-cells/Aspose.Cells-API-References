---
title: "Enum HeaderFooterCommandType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.HeaderFooterCommandType. Rappresenta il tipo di comando dell'intestazione e del piè di pagina"
type: docs
url: /it/net/aspose.cells/headerfootercommandtype/
---
## HeaderFooterCommandType enumeration

Rappresenta il tipo di comando dell'intestazione e del piè di pagina.

```csharp
public enum HeaderFooterCommandType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Text | `0` | Il testo. |
| CurrentPage | `1` | Numero di pagina corrente |
| Pagecount | `2` | Conteggio pagine |
| CurrentDate | `3` | Data corrente |
| CurrentTime | `4` | Ora corrente |
| SheetName | `5` | Nome del foglio |
| FileName | `6` | Nome file senza percorso |
| FilePath | `7` | Percorso file senza nome file |
| Picture | `8` | Immagine |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHeaderFooterCommandTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Imposta l'intestazione con diversi tipi di comando
                worksheet.PageSetup.SetHeader(0, "&[Page] of &[Pages] - &[Date] - &[Time] - &[File]");

                // Recupera i comandi dell'intestazione
                string headerScript = worksheet.PageSetup.GetHeader(0);
                HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(headerScript);

                // Dimostra i diversi valori di HeaderFooterCommandType
                foreach (HeaderFooterCommand cmd in commands)
                {
                    Console.WriteLine($"Command Type: {cmd.Type}");

                    // Verifica tipi di comando specifici
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

                // Salva la cartella di lavoro per dimostrare la configurazione dell'intestazione
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

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


