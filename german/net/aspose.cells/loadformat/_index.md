---
title: "Aufzählung LoadFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LoadFormat Aufzählung. Stellt das Lade-Dateiformat dar."
type: docs
url: /de/net/aspose.cells/loadformat/
---
## LoadFormat enumeration

Stellt das Lade-Dateiformat dar.

```csharp
public enum LoadFormat
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Auto | `0` | Stellt die automatische Erkennung des Formats dar. |
| Csv | `1` | Kommagetrennte Werte (CSV) Textdatei. |
| CSV | `1` | Kommagetrennte Werte (CSV) Textdatei. HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Csv‑Eigenschaft. Diese Eigenschaft wird 6 Monate nach April 2021 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben. |
| Xlsx | `6` | Stellt ein Office Open XML spreadsheetML Arbeitsbuch oder eine Vorlage dar, mit oder ohne Makros. |
| Tsv | `11` | Tabulatorgetrennte Werte (TSV) Textdatei. |
| TSV | `11` | Tabulatorgetrennte Werte (TSV) Textdatei. HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Tsv‑Eigenschaft. Diese Eigenschaft wird 6 Monate nach April 2021 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben. |
| TabDelimited | `11` | Stellt eine tabulatorgetrennte Textdatei dar, gleich wie Tsv. |
| Html | `12` | Stellt eine html-Datei dar. |
| MHtml | `13` | Stellt eine mhtml-Datei dar. |
| Ods | `14` | Open Document Sheet(ODS)-Datei. |
| ODS | `14` | Open Document Sheet(ODS)-Datei. HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Ods property. Diese property wird 6 Monate später seit April 2021 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben. |
| Excel97To2003 | `5` | Stellt eine Excel97-2003 xls-Datei dar. |
| SpreadsheetML | `15` | Stellt eine Excel 2003 xml-Datei dar. |
| Xlsb | `16` | Stellt eine xlsb-Datei dar. |
| Ots | `31` | Open Document Template Sheet(OTS)-Datei. |
| Numbers | `56` | Stellt eine numbers-Datei dar. |
| Fods | `59` | Stellt das OpenDocument Flat XML Spreadsheet (.fods)-Dateiformat dar. |
| FODS | `59` | Stellt das OpenDocument Flat XML Spreadsheet (.fods)-Dateiformat dar. HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Fods property. Diese property wird 6 Monate später seit April 2021 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben. |
| Sxc | `60` | Stellt das StarOffice Calc Spreadsheet (.sxc)-Dateiformat dar. |
| SXC | `60` | Stellt das StarOffice Calc Spreadsheet (.sxc)-Dateiformat dar. HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Sxc property. Diese property wird 6 Monate später seit April 2021 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben. |
| Xml | `51` | Stellt eine einfache xml-Datei dar. |
| Epub | `52` | Stellt eine EPUB-Datei dar. |
| Azw3 | `53` | Stellt eine AZW3-Datei dar. |
| Chm | `54` | Stellt eine CHM-Datei dar. |
| Markdown | `55` | Stellt eine Markdown-Datei dar. |
| Unknown | `255` | Stellt ein nicht erkanntes Format dar, kann nicht geladen werden. |
| Image | `254` | Bild |
| Json | `513` | Json |
| Dif | `30` | Daten-Austauschformat. |
| Dbf | `515` | Xbase-Datendatei |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFormatDemo
    {
        public static void LoadFormatExample()
        {
            // Laden Sie eine Excel-Datei in verschiedenen Formaten mit Aspose.Cells
            string[] filePaths = {
                "LoadFormatDemo_original.xlsx",
                "LoadFormatDemo_original.xls",
                "LoadFormatDemo_original.csv",
                "LoadFormatDemo_original.json"
            };

            foreach (var filePath in filePaths)
            {
                // Bestimmen Sie das Ladeformat basierend auf der Dateierweiterung
                LoadFormat loadFormat = GetLoadFormat(filePath);

                // Erstelle LoadOptions mit dem ermittelten LoadFormat
                LoadOptions loadOptions = new LoadOptions(loadFormat);

                // Lade die Arbeitsmappe mit den angegebenen Ladeoptionen
                Workbook workbook = new Workbook(filePath, loadOptions);

                // Führe einige Vorgänge mit der Arbeitsmappe aus
                Console.WriteLine($"Loaded file: {filePath}");
                Console.WriteLine($"Number of sheets: {workbook.Worksheets.Count}");

                // Speichere die Arbeitsmappe in einer neuen Datei
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

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


