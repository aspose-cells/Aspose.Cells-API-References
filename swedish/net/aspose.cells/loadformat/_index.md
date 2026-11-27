---
title: "Enum LoadFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LoadFormat‑enum. Representerar filformatet för inläsning"
type: docs
url: /sv/net/aspose.cells/loadformat/
---
## LoadFormat enumeration

Representerar filformatet för inläsning.

```csharp
public enum LoadFormat
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Auto | `0` | Representerar att formatet identifieras automatiskt. |
| Csv | `1` | Kommaseparerade värden (CSV) textfil. |
| CSV | `1` | Kommaseparerade värden (CSV) textfil. OBS: Denna medlem är nu föråldrad. Använd istället Csv‑egenskapen. Denna egenskap kommer att tas bort 6 månader senare från och med april 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. |
| Xlsx | `6` | Representerar Office Open XML spreadsheetML-arbetsbok eller mall, med eller utan makron. |
| Tsv | `11` | Tabbseparerade värden (TSV) textfil. |
| TSV | `11` | Tabbseparerade värden (TSV) textfil. OBS: Denna medlem är nu föråldrad. Använd istället Tsv‑egenskapen. Denna egenskap kommer att tas bort 6 månader senare från och med april 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. |
| TabDelimited | `11` | Representerar en tabbavgränsad textfil, samma som Tsv. |
| Html | `12` | Representerar en HTML‑fil. |
| MHtml | `13` | Representerar en MHTML‑fil. |
| Ods | `14` | Open Document Sheet (ODS)-fil. |
| ODS | `14` | Open Document Sheet (ODS)-fil. OBS: Denna medlem är nu föråldrad. Använd istället Ods‑egenskapen. Denna egenskap kommer att tas bort 6 månader senare från och med april 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. |
| Excel97To2003 | `5` | Representerar en Excel97-2003 xls‑fil. |
| SpreadsheetML | `15` | Representerar en Excel 2003 xml‑fil. |
| Xlsb | `16` | Representerar en xlsb‑fil. |
| Ots | `31` | Open Document Template Sheet (OTS)-fil. |
| Numbers | `56` | Representerar en Numbers‑fil. |
| Fods | `59` | Representerar OpenDocument Flat XML Spreadsheet (.fods)-filformat. |
| FODS | `59` | Representerar OpenDocument Flat XML Spreadsheet (.fods)-filformat. OBS: Denna medlem är nu föråldrad. Använd istället Fods‑egenskapen. Denna egenskap kommer att tas bort 6 månader senare från och med april 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. |
| Sxc | `60` | Representerar StarOffice Calc Spreadsheet (.sxc)-filformat. |
| SXC | `60` | Representerar StarOffice Calc Spreadsheet (.sxc)-filformat. OBS: Denna medlem är nu föråldrad. Använd istället Sxc‑egenskapen. Denna egenskap kommer att tas bort 6 månader senare från och med april 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. |
| Xml | `51` | Representerar en enkel xml-fil. |
| Epub | `52` | Representerar en EPUB-fil. |
| Azw3 | `53` | Representerar en AZW3-fil. |
| Chm | `54` | Representerar en CHM-fil. |
| Markdown | `55` | Representerar en Markdown-fil. |
| Unknown | `255` | Representerar ett okänt format, kan inte laddas. |
| Image | `254` | Bild |
| Json | `513` | Json |
| Dif | `30` | Datautbytesformat. |
| Dbf | `515` | Xbase-datafil |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFormatDemo
    {
        public static void LoadFormatExample()
        {
            // Läs in en Excel-fil i olika format med Aspose.Cells
            string[] filePaths = {
                "LoadFormatDemo_original.xlsx",
                "LoadFormatDemo_original.xls",
                "LoadFormatDemo_original.csv",
                "LoadFormatDemo_original.json"
            };

            foreach (var filePath in filePaths)
            {
                // Bestäm inläsningsformatet baserat på filändelsen
                LoadFormat loadFormat = GetLoadFormat(filePath);

                // Skapa LoadOptions med det bestämda LoadFormat
                LoadOptions loadOptions = new LoadOptions(loadFormat);

                // Läs in arbetsboken med de angivna inläsningsalternativen
                Workbook workbook = new Workbook(filePath, loadOptions);

                // Utför några operationer på arbetsboken
                Console.WriteLine($"Loaded file: {filePath}");
                Console.WriteLine($"Number of sheets: {workbook.Worksheets.Count}");

                // Spara arbetsboken till en ny fil
                string outputFilePath = $"output_{System.IO.Path.GetFileName(filePath)}";
                workbook.Save(outputFilePath);
                Console.WriteLine($"Saved file as: {outputFilePath}");
            }
        }

        private static LoadFormat GetLoadFormat(string filePath)
        {
            string extension = System.IO.Path.GetExtension(filePath).ToLower();
            switch (extension)
            {
                case ".xlsx":
                    return LoadFormat.Xlsx;
                case ".xls":
                    return LoadFormat.Excel97To2003;
                case ".csv":
                    return LoadFormat.Csv;
                case ".json":
                    return LoadFormat.Json;
                default:
                    return LoadFormat.Auto;
            }
        }
    }

}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


