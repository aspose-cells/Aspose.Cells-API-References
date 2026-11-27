---
title: "Enum FileFormatType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FileFormatType enum. Representerar filformattyperna"
type: docs
url: /sv/net/aspose.cells/fileformattype/
---
## FileFormatType enumeration

Representerar filformattyperna.

```csharp
public enum FileFormatType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Csv | `1` | Kommaseparerade värden (CSV) textfil. |
| Xlsx | `6` | Office Open XML SpreadsheetML-fil (utan makron). |
| Xlsm | `7` | Office Open XML SpreadsheetML-fil med makron. |
| Xltx | `8` | Office Open XML SpreadsheetML-mall (utan makron). |
| Xltm | `9` | Office Open XML SpreadsheetML-mall med makron. |
| Xlam | `10` | Office Open XML SpreadsheetML-tilläggsfil med makron. |
| Tsv | `11` | Tabbseparerade värden (TSV) textfil. |
| TabDelimited | `11` | Tab-separerade värden (TSV) textfil, samma som Tsv. |
| Html | `12` | HTML-format. |
| MHtml | `17` | MHTML (webarkiv) format. |
| Ods | `14` | Open Document Sheet (ODS)-fil. |
| Excel97To2003 | `5` | Excel97-2003 kalkylbladsfil. |
| SpreadsheetML | `15` | Excel 2003 XML-datafil. |
| Xlsb | `16` | Det binära Excel-filformatet (.xlsb) |
| Unknown | `255` | Representerar ett okänt format, kan inte laddas. |
| Pdf | `13` | PDF (Adobe Portable Document) format. |
| Xps | `20` | XPS (XML Paper Specification)-format. |
| Tiff | `21` | Representerar en TIFF-fil. |
| Svg | `28` | SVG-fil. |
| Excel95 | `22` | Representerar en Excel95 xls-fil. |
| Excel4 | `23` | Representerar en Excel4.0 xls-fil. |
| Excel3 | `24` | Representerar en Excel3.0 xls-fil. |
| Excel2 | `25` | Representerar en Excel2.1 xls-fil. |
| Pptx | `26` | Representerar en pptx-fil. |
| Docx | `27` | Representerar en docx-fil. |
| Dif | `30` | Datautbytesformat. |
| Doc | `31` | Representerar en doc-fil. |
| Ppt | `32` | Representerar en ppt-fil. |
| MapiMessage | `33` | Representerar en e-postfil. |
| MsEquation | `34` | Representerar MS Equation 3.0-objektet. |
| Ole10Native | `35` | Representerar det inbäddade inhemska objektet. |
| Vsd | `36` | Representerar MS Visio VSD-binärformatet. |
| Vsdx | `37` | Representerar MS Visio 2013 VSDX-filformatet. |
| Docm | `38` | Representerar en docm-fil. |
| Dotx | `39` | Representerar en dotx-fil. |
| Dotm | `40` | Representerar en dotm-fil. |
| Pptm | `41` | Representerar en pptm-fil. |
| Potx | `42` | Representerar en Potx-fil. |
| Potm | `43` | Representerar en Potm-fil. |
| Ppsx | `44` | Representerar en ppsx-fil. |
| Ppsm | `45` | Representerar en ppsm-fil. |
| Ooxml | `46` | Representerar Office Open XML-fil (såsom xlsx, docx, pptx, etc). |
| Odt | `47` | Representerar en ODT-fil. |
| Odp | `48` | Representerar en ODP-fil. |
| Odf | `49` | Representerar en ODF-fil. |
| Odg | `50` | Representerar en ODG-fil. |
| Xml | `51` | Representerar en enkel xml-fil. |
| Xlt | `52` | Excel97-2003 kalkylbladsmall. |
| Ott | `53` | Representerar en OTT-fil. |
| Bmp | `54` | Representerar en BMP-fil. |
| Ots | `55` | Representerar en ots-fil. |
| Numbers | `56` | Representerar Numbers 9.0-filformatet från Apple Inc. |
| Numbers09 | `56` | Representerar Numbers 9.0-filformatet från Apple Inc. |
| Markdown | `57` | Representerar ett markdown-dokument. |
| GraphChart | `58` | Representerar inbäddat diagram. |
| Fods | `59` | Representerar OpenDocument Flat XML Spreadsheet (.fods)-filformat. |
| Sxc | `60` | Representerar StarOffice Calc Spreadsheet (.sxc)-filformat. |
| Otp | `61` | Representerar en OTP-fil. |
| Numbers35 | `62` | Representerar Numbers 3.5-filformatet sedan 2014 från Apple Inc |
| Ole | `64` | Representerar det inbäddade ole-objektet. |
| Emf | `258` | Windows Enhanced Metafile. |
| Wmf | `259` | Windows Metafil. |
| Jpg | `261` | JPEG JFIF. |
| Png | `262` | Portable Network Graphics. |
| Gif | `322` | Gif |
| WebP | `323` | Webp |
| Json | `513` | Json |
| SqlScript | `514` | Sql |
| Dbf | `515` | Xbase-datafil |
| FlatOpc | `516` | Flat opc-fil |
| XHtml | `771` | Representerar XHtml-fil. |
| OneNote | `772` | Representerar One Note-fil. |
| MicrosoftCabinet | `773` | Representerar Microsoft Cabinet-fil. |
| Rtf | `774` | Rtf |
| Epub | `775` | EPUB |
| Azw3 | `777` | AZW3 |
| Chm | `784` | CHM |
| Oxps | `776` | OXPS (Open XML Paper Specification) format. |
| GZip | `35615` | Representerar GZip-fil. |
| Otg | `1025` | Representerar en OTG-fil. |
| Odb | `1026` | Representerar en Odb-fil. |
| Ofd | `1029` | Representerar en Ofd-fil. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatTypeDemo
    {
        public static void FileFormatTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange namnet på arbetsbladet
            worksheet.Name = "File Format Example";

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("File Format Type");
            worksheet.Cells["A2"].PutValue(FileFormatType.Csv);
            worksheet.Cells["A3"].PutValue(FileFormatType.Xlsx);
            worksheet.Cells["A4"].PutValue(FileFormatType.Pdf);
            worksheet.Cells["A5"].PutValue(FileFormatType.Xlsm);

            // Skriv ut filformattyperna
            for (int i = 2; i <= 5; i++)
            {
                var fileFormat = worksheet.Cells[$"A{i}"].StringValue;
                Console.WriteLine($"Row {i}: {fileFormat}");
            }

            // Spara arbetsboken
            workbook.Save("FileFormatTypeExample.xlsx");
            workbook.Save("FileFormatTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


