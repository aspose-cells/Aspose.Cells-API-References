---
title: "Enum FileFormatType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.FileFormatType enum. Rappresenta i tipi di formato file"
type: docs
url: /it/net/aspose.cells/fileformattype/
---
## FileFormatType enumeration

Rappresenta i tipi di formato file.

```csharp
public enum FileFormatType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Csv | `1` | File di testo CSV (valori separati da virgola). |
| Xlsx | `6` | File Office Open XML SpreadsheetML (senza macro). |
| Xlsm | `7` | File Office Open XML SpreadsheetML abilitato alle macro. |
| Xltx | `8` | Modello Office Open XML SpreadsheetML (senza macro). |
| Xltm | `9` | Modello Office Open XML SpreadsheetML abilitato alle macro. |
| Xlam | `10` | File Office Open XML SpreadsheetML addinMacro-Enabled. |
| Tsv | `11` | File di testo TSV (valori separati da tabulazione). |
| TabDelimited | `11` | File di testo Tab-Separated Values (TSV), stesso di Tsv. |
| Html | `12` | Formato HTML. |
| MHtml | `17` | Formato MHTML (archivio Web). |
| Ods | `14` | File Open Document Sheet (ODS). |
| Excel97To2003 | `5` | File di foglio di calcolo Excel97-2003. |
| SpreadsheetML | `15` | File di dati XML Excel 2003. |
| Xlsb | `16` | Il formato di file binario Excel (.xlsb). |
| Unknown | `255` | Rappresenta un formato non riconosciuto, impossibile da caricare. |
| Pdf | `13` | Formato PDF (Adobe Portable Document). |
| Xps | `20` | Formato XPS (XML Paper Specification). |
| Tiff | `21` | Rappresenta un file TIFF. |
| Svg | `28` | File SVG. |
| Excel95 | `22` | Rappresenta un file Excel95 xls. |
| Excel4 | `23` | Rappresenta un file Excel4.0 xls. |
| Excel3 | `24` | Rappresenta un file Excel3.0 xls. |
| Excel2 | `25` | Rappresenta un file Excel2.1 xls. |
| Pptx | `26` | Rappresenta un file pptx. |
| Docx | `27` | Rappresenta un file docx. |
| Dif | `30` | Formato di scambio dati. |
| Doc | `31` | Rappresenta un file doc. |
| Ppt | `32` | Rappresenta un file ppt. |
| MapiMessage | `33` | Rappresenta un file email. |
| MsEquation | `34` | Rappresenta l'oggetto MS Equation 3.0. |
| Ole10Native | `35` | Rappresenta l'oggetto nativo incorporato. |
| Vsd | `36` | Rappresenta il formato binario MS Visio VSD. |
| Vsdx | `37` | Rappresenta il formato file MS Visio 2013 VSDX. |
| Docm | `38` | Rappresenta un file docm. |
| Dotx | `39` | Rappresenta un file dotx. |
| Dotm | `40` | Rappresenta un file dotm. |
| Pptm | `41` | Rappresenta un file pptm. |
| Potx | `42` | Rappresenta un file Potx. |
| Potm | `43` | Rappresenta un file Potm. |
| Ppsx | `44` | Rappresenta un file ppsx. |
| Ppsm | `45` | Rappresenta un file ppsm. |
| Ooxml | `46` | Rappresenta un file Office Open XML (come xlsx, docx, pptx, ecc). |
| Odt | `47` | Rappresenta un file ODT. |
| Odp | `48` | Rappresenta un file ODP. |
| Odf | `49` | Rappresenta un file ODF. |
| Odg | `50` | Rappresenta un file ODG. |
| Xml | `51` | Rappresenta un file XML semplice. |
| Xlt | `52` | Modello di foglio di calcolo Excel97-2003. |
| Ott | `53` | Rappresenta un file OTT. |
| Bmp | `54` | Rappresenta un file BMP. |
| Ots | `55` | Rappresenta un file ots. |
| Numbers | `56` | Rappresenta il formato file Numbers 9.0 di Apple Inc. |
| Numbers09 | `56` | Rappresenta il formato file Numbers 9.0 di Apple Inc. |
| Markdown | `57` | Rappresenta un documento markdown. |
| GraphChart | `58` | Rappresenta un grafico incorporato. |
| Fods | `59` | Rappresenta il formato di file OpenDocument Flat XML Spreadsheet (.fods). |
| Sxc | `60` | Rappresenta il formato di file StarOffice Calc Spreadsheet (.sxc). |
| Otp | `61` | Rappresenta un file OTP. |
| Numbers35 | `62` | Rappresenta il formato file Numbers 3.5, dal 2014, di Apple Inc. |
| Ole | `64` | Rappresenta l'oggetto OLE incorporato. |
| Emf | `258` | Metafile migliorato di Windows. |
| Wmf | `259` | Metafile Windows. |
| Jpg | `261` | JPEG JFIF. |
| Png | `262` | Grafica di rete portatile. |
| Gif | `322` | Gif |
| WebP | `323` | Webp |
| Json | `513` | Json |
| SqlScript | `514` | Sql |
| Dbf | `515` | File dati Xbase |
| FlatOpc | `516` | File OPC flat |
| XHtml | `771` | Rappresenta il file XHtml. |
| OneNote | `772` | Rappresenta il file One Note. |
| MicrosoftCabinet | `773` | Rappresenta il file Microsoft Cabinet. |
| Rtf | `774` | Rtf |
| Epub | `775` | EPUB |
| Azw3 | `777` | AZW3 |
| Chm | `784` | CHM |
| Oxps | `776` | Formato OXPS (Open XML Paper Specification). |
| GZip | `35615` | Rappresenta il file GZip. |
| Otg | `1025` | Rappresenta un file OTG. |
| Odb | `1026` | Rappresenta un file Odb. |
| Ofd | `1029` | Rappresenta un file Ofd. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatTypeDemo
    {
        public static void FileFormatTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta il nome del foglio di lavoro
            worksheet.Name = "File Format Example";

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("File Format Type");
            worksheet.Cells["A2"].PutValue(FileFormatType.Csv);
            worksheet.Cells["A3"].PutValue(FileFormatType.Xlsx);
            worksheet.Cells["A4"].PutValue(FileFormatType.Pdf);
            worksheet.Cells["A5"].PutValue(FileFormatType.Xlsm);

            // Restituisce i tipi di formato file
            for (int i = 2; i <= 5; i++)
            {
                var fileFormat = worksheet.Cells[$"A{i}"].StringValue;
                Console.WriteLine($"Row {i}: {fileFormat}");
            }

            // Salva la cartella di lavoro
            workbook.Save("FileFormatTypeExample.xlsx");
            workbook.Save("FileFormatTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


