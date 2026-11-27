---
title: "Enum SaveFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.SaveFormat enum. Representerar formatet som arbetsboken sparas i"
type: docs
url: /sv/net/aspose.cells/saveformat/
---
## SaveFormat enumeration

Representerar formatet som arbetsboken sparas i.

```csharp
public enum SaveFormat
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Csv | `1` | Kommaseparerade värden (CSV) textfil. |
| CSV | `1` | Kommaseparerade värden (CSV) textfil. OBS: Denna medlem är nu föråldrad. Använd istället Csv‑egenskapen. Denna egenskap kommer att tas bort 6 månader senare från och med april 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. |
| Xlsx | `6` | Representerar en xlsx-fil. |
| Xlsm | `7` | Representerar en xlsm-fil som möjliggör makron. |
| Xltx | `8` | Representerar en xltx-fil. |
| Xltm | `9` | Representerar en xltm-fil som möjliggör makron. |
| Xlam | `10` | Representerar en xltm-fil som möjliggör tilläggsmakron. |
| Tsv | `11` | Tabbseparerade värden (TSV) textfil. |
| TSV | `11` | Tabbseparerade värden (TSV) textfil. OBS: Denna medlem är nu föråldrad. Använd istället Tsv‑egenskapen. Denna egenskap kommer att tas bort 6 månader senare från och med april 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. |
| TabDelimited | `11` | Representerar en tabbavgränsad textfil, samma som Tsv. |
| Html | `12` | Representerar en HTML‑fil. |
| MHtml | `17` | Representerar en MHTML‑fil. |
| Ods | `14` | Open Document Sheet (ODS)-fil. |
| ODS | `14` | Open Document Sheet (ODS)-fil. OBS: Denna medlem är nu föråldrad. Använd istället Ods‑egenskapen. Denna egenskap kommer att tas bort 6 månader senare från och med april 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. |
| Excel97To2003 | `5` | Representerar en Excel97-2003 xls‑fil. |
| SpreadsheetML | `15` | Representerar en Excel 2003 xml‑fil. |
| Xlsb | `16` | Representerar en xlsb‑fil. |
| Auto | `0` | Om du sparar filen till disken, följer filformatet filnamnets filändelse. Om du sparar filen till strömmen, är filformatet xlsx. |
| Unknown | `255` | Representerar ett okänt format, kan inte sparas. |
| Pdf | `13` | Representerar en PDF-fil. |
| Xps | `20` | XPS (XML Paper Specification)-format. |
| XPS | `20` | XPS (XML Paper Specification)-format. OBS! Denna medlem är nu föråldrad. Använd istället Xps-egenskapen. Denna egenskap kommer att tas bort 6 månader senare sedan april 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. |
| Tiff | `21` | Representerar en TIFF-fil. |
| TIFF | `21` | Representerar en TIFF-fil. OBS! Denna medlem är nu föråldrad. Använd istället Tiff-egenskapen. Denna egenskap kommer att tas bort 6 månader senare sedan april 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. |
| Svg | `28` | SVG-fil. |
| SVG | `28` | SVG-fil. OBS! Denna medlem är nu föråldrad. Använd istället Svg-egenskapen. Denna egenskap kommer att tas bort 6 månader senare sedan april 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. |
| Dif | `30` | Datautbytesformat. |
| Ots | `31` | Open Document Template Sheet (OTS)-fil. |
| Xlt | `32` | Excel 97-2003-mallfil. |
| Xml | `51` | Representerar en enkel xml-fil. |
| Numbers | `56` | Representerar en Numbers-fil sedan 2014 av Apple Inc. |
| Markdown | `57` | Representerar ett markdown-dokument. |
| Fods | `59` | Representerar OpenDocument Flat XML Spreadsheet (.fods)-filformat. |
| FODS | `59` | Representerar OpenDocument Flat XML Spreadsheet (.fods)-filformat. OBS: Denna medlem är nu föråldrad. Använd istället Fods‑egenskapen. Denna egenskap kommer att tas bort 6 månader senare från och med april 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. |
| Sxc | `60` | Representerar StarOffice Calc Spreadsheet (.sxc)-filformat. |
| SXC | `60` | Representerar StarOffice Calc Spreadsheet (.sxc)-filformat. OBS: Denna medlem är nu föråldrad. Använd istället Sxc‑egenskapen. Denna egenskap kommer att tas bort 6 månader senare från och med april 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. |
| Pptx | `61` | Representerar en .pptx-fil. |
| Docx | `62` | Representerar en .docx-fil. |
| Emf | `258` | Windows Enhanced Metafile. |
| Jpg | `261` | JPEG JFIF. |
| Png | `262` | Portable Network Graphics. |
| Bmp | `263` | Windows Bitmap |
| Gif | `322` | Gif |
| Json | `513` | Json |
| SqlScript | `514` | Sql |
| XHtml | `771` | Representerar XHtml-fil. vänligen använd [`HtmlVersion`](../htmlsaveoptions/htmlversion/) egenskap. Denna egenskap kommer att tas bort 6 månader senare, sedan mars 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. |
| Epub | `772` | Representerar Epub-fil. |
| Azw3 | `773` | Representerar Azw3-fil. |
| Pcl | `1025` | PCL (Skrivarens kommandospråk) |
| Ofd | `1026` | OFD (Öppet fastlayout-dokument) |
| Dbf | `515` | Xbase-datafil |

### Exempel

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class SaveFormatDemo
    {
        public static void SaveFormatExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Spara arbetsboken i olika format
            workbook.Save("SaveFormatExample.xlsx", SaveFormat.Xlsx);
            workbook.Save("SaveFormatExample.xls", SaveFormat.Excel97To2003);
            workbook.Save("SaveFormatExample.csv", SaveFormat.Csv);
            workbook.Save("SaveFormatExample.pdf", SaveFormat.Pdf);
            workbook.Save("SaveFormatExample.html", SaveFormat.Html);

            // Skriv ut resultaten
            Console.WriteLine("Workbook saved in multiple formats.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


