---
title: "Enum SaveFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.SaveFormat. Rappresenta il formato in cui la cartella di lavoro viene salvata"
type: docs
url: /it/net/aspose.cells/saveformat/
---
## SaveFormat enumeration

Rappresenta il formato in cui la cartella di lavoro è salvata.

```csharp
public enum SaveFormat
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Csv | `1` | File di testo CSV (valori separati da virgola). |
| CSV | `1` | File di testo CSV (valori separati da virgola). NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Csv. Questa proprietà sarà rimossa 6 mesi dopo, a partire da aprile 2021. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato. |
| Xlsx | `6` | Rappresenta un file xlsx. |
| Xlsm | `7` | Rappresenta un file xlsm che abilita le macro. |
| Xltx | `8` | Rappresenta un file xltx. |
| Xltm | `9` | Rappresenta un file xltm che abilita le macro. |
| Xlam | `10` | Rappresenta un file xltm che abilita le macro di componenti aggiuntivi. |
| Tsv | `11` | File di testo TSV (valori separati da tabulazione). |
| TSV | `11` | File di testo TSV (valori separati da tabulazione). NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Tsv. Questa proprietà sarà rimossa 6 mesi dopo, a partire da aprile 2021. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato. |
| TabDelimited | `11` | Rappresenta un file di testo delimitato da tabulazione, uguale a Tsv. |
| Html | `12` | Rappresenta un file HTML. |
| MHtml | `17` | Rappresenta un file MHTML. |
| Ods | `14` | File Open Document Sheet (ODS). |
| ODS | `14` | File Open Document Sheet (ODS). NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Ods. Questa proprietà sarà rimossa 6 mesi dopo, a partire da aprile 2021. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato. |
| Excel97To2003 | `5` | Rappresenta un file Excel97-2003 xls. |
| SpreadsheetML | `15` | Rappresenta un file Excel 2003 xml. |
| Xlsb | `16` | Rappresenta un file xlsb. |
| Auto | `0` | Se si salva il file su disco, il formato del file corrisponde all'estensione del nome file. Se si salva il file su stream, il formato del file è xlsx. |
| Unknown | `255` | Rappresenta un formato non riconosciuto, non può essere salvato. |
| Pdf | `13` | Rappresenta un file PDF. |
| Xps | `20` | Formato XPS (XML Paper Specification). |
| XPS | `20` | Formato XPS (XML Paper Specification). NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Xps. Questa proprietà sarà rimossa 6 mesi dopo, a partire da aprile 2021. Aspose si scusa per eventuali disagi che potresti aver riscontrato. |
| Tiff | `21` | Rappresenta un file TIFF. |
| TIFF | `21` | Rappresenta un file TIFF. NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Tiff. Questa proprietà sarà rimossa 6 mesi dopo, a partire da aprile 2021. Aspose si scusa per eventuali disagi che potresti aver riscontrato. |
| Svg | `28` | File SVG. |
| SVG | `28` | File SVG. NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Svg. Questa proprietà sarà rimossa 6 mesi dopo, a partire da aprile 2021. Aspose si scusa per eventuali disagi che potresti aver riscontrato. |
| Dif | `30` | Formato di scambio dati. |
| Ots | `31` | File Open Document Template Sheet (OTS). |
| Xlt | `32` | File modello Excel 97-2003. |
| Xml | `51` | Rappresenta un file XML semplice. |
| Numbers | `56` | Rappresenta un file Numbers di Apple Inc. dal 2014. |
| Markdown | `57` | Rappresenta un documento markdown. |
| Fods | `59` | Rappresenta il formato di file OpenDocument Flat XML Spreadsheet (.fods). |
| FODS | `59` | Rappresenta il formato di file OpenDocument Flat XML Spreadsheet (.fods). NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Fods. Questa proprietà sarà rimossa 6 mesi dopo, a partire da aprile 2021. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato. |
| Sxc | `60` | Rappresenta il formato di file StarOffice Calc Spreadsheet (.sxc). |
| SXC | `60` | Rappresenta il formato di file StarOffice Calc Spreadsheet (.sxc). NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Sxc. Questa proprietà sarà rimossa 6 mesi dopo, a partire da aprile 2021. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato. |
| Pptx | `61` | Rappresenta un file .pptx. |
| Docx | `62` | Rappresenta un file .docx. |
| Emf | `258` | Metafile migliorato di Windows. |
| Jpg | `261` | JPEG JFIF. |
| Png | `262` | Grafica di rete portatile. |
| Bmp | `263` | Bitmap di Windows |
| Gif | `322` | Gif |
| Json | `513` | Json |
| SqlScript | `514` | Sql |
| XHtml | `771` | Rappresenta un file XHtml. Si prega di utilizzare la proprietà [`HtmlVersion`](../htmlsaveoptions/htmlversion/). Questa proprietà sarà rimossa tra 6 mesi a partire da marzo 2025. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato. |
| Epub | `772` | Rappresenta un file Epub. |
| Azw3 | `773` | Rappresenta un file Azw3. |
| Pcl | `1025` | PCL (Printer Command Language) |
| Ofd | `1026` | OFD (Open Fixed-layout Document) |
| Dbf | `515` | File dati Xbase |

### Esempi

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class SaveFormatDemo
    {
        public static void SaveFormatExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Salva la cartella di lavoro in diversi formati
            workbook.Save("SaveFormatExample.xlsx", SaveFormat.Xlsx);
            workbook.Save("SaveFormatExample.xls", SaveFormat.Excel97To2003);
            workbook.Save("SaveFormatExample.csv", SaveFormat.Csv);
            workbook.Save("SaveFormatExample.pdf", SaveFormat.Pdf);
            workbook.Save("SaveFormatExample.html", SaveFormat.Html);

            // Restituisci i risultati
            Console.WriteLine("Workbook saved in multiple formats.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


