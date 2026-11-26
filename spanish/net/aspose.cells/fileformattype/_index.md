---
title: "Enumeración FileFormatType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.FileFormatType. Representa los tipos de formato de archivo"
type: docs
url: /es/net/aspose.cells/fileformattype/
---
## FileFormatType enumeration

Representa los tipos de formato de archivo.

```csharp
public enum FileFormatType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Csv | `1` | Archivo de texto de valores separados por comas (CSV). |
| Xlsx | `6` | Archivo Office Open XML SpreadsheetML (sin macros). |
| Xlsm | `7` | Archivo Office Open XML SpreadsheetML con macros habilitadas. |
| Xltx | `8` | Plantilla Office Open XML SpreadsheetML (sin macros). |
| Xltm | `9` | Plantilla Office Open XML SpreadsheetML con macros habilitadas. |
| Xlam | `10` | Archivo Office Open XML SpreadsheetML addin habilitado para macros. |
| Tsv | `11` | Archivo de texto de valores separados por tabulaciones (TSV). |
| TabDelimited | `11` | Archivo de texto de valores separados por tabulaciones (TSV), lo mismo con Tsv. |
| Html | `12` | Formato HTML. |
| MHtml | `17` | Formato MHTML (archivo web). |
| Ods | `14` | Archivo Open Document Sheet (ODS). |
| Excel97To2003 | `5` | Archivo de hoja de cálculo Excel97-2003. |
| SpreadsheetML | `15` | Archivo de datos XML de Excel 2003. |
| Xlsb | `16` | El formato de archivo binario de Excel (.xlsb) |
| Unknown | `255` | Representa un formato no reconocido, no se puede cargar. |
| Pdf | `13` | Formato PDF (Documento portátil de Adobe). |
| Xps | `20` | Formato XPS (XML Paper Specification). |
| Tiff | `21` | Representa un archivo TIFF. |
| Svg | `28` | Archivo SVG. |
| Excel95 | `22` | Representa un archivo Excel95 xls. |
| Excel4 | `23` | Representa un archivo Excel4.0 xls. |
| Excel3 | `24` | Representa un archivo Excel3.0 xls. |
| Excel2 | `25` | Representa un archivo Excel2.1 xls. |
| Pptx | `26` | Representa un archivo pptx. |
| Docx | `27` | Representa un archivo docx. |
| Dif | `30` | Formato de Intercambio de Datos. |
| Doc | `31` | Representa un archivo doc. |
| Ppt | `32` | Representa un archivo ppt. |
| MapiMessage | `33` | Representa un archivo de correo electrónico. |
| MsEquation | `34` | Representa el objeto MS Equation 3.0. |
| Ole10Native | `35` | Representa el objeto nativo incrustado. |
| Vsd | `36` | Representa el formato binario MS Visio VSD. |
| Vsdx | `37` | Representa el formato de archivo MS Visio 2013 VSDX. |
| Docm | `38` | Representa un archivo docm. |
| Dotx | `39` | Representa un archivo dotx. |
| Dotm | `40` | Representa un archivo dotm. |
| Pptm | `41` | Representa un archivo pptm. |
| Potx | `42` | Representa un archivo Potx. |
| Potm | `43` | Representa un archivo Potm. |
| Ppsx | `44` | Representa un archivo ppsx. |
| Ppsm | `45` | Representa un archivo ppsm. |
| Ooxml | `46` | Representa un archivo office open xml (como xlsx, docx, pptx, etc). |
| Odt | `47` | Representa un archivo ODT. |
| Odp | `48` | Representa un archivo ODP. |
| Odf | `49` | Representa un archivo ODF. |
| Odg | `50` | Representa un archivo ODG. |
| Xml | `51` | Representa un archivo xml simple. |
| Xlt | `52` | Plantilla de hoja de cálculo Excel97-2003. |
| Ott | `53` | Representa un archivo OTT. |
| Bmp | `54` | Representa un archivo BMP. |
| Ots | `55` | Representa un archivo ots. |
| Numbers | `56` | Representa el formato de archivo Numbers 9.0 de Apple Inc. |
| Numbers09 | `56` | Representa el formato de archivo Numbers 9.0 de Apple Inc. |
| Markdown | `57` | Representa un documento markdown. |
| GraphChart | `58` | Representa un gráfico incrustado. |
| Fods | `59` | Representa el formato de archivo OpenDocument Flat XML Spreadsheet (.fods). |
| Sxc | `60` | Representa el formato de archivo StarOffice Calc Spreadsheet (.sxc). |
| Otp | `61` | Representa un archivo OTP. |
| Numbers35 | `62` | Representa el formato de archivo Numbers 3.5 desde 2014 de Apple Inc. |
| Ole | `64` | Representa el objeto ole incrustado. |
| Emf | `258` | Metarchivo mejorado de Windows. |
| Wmf | `259` | Metarchivo de Windows. |
| Jpg | `261` | JPEG JFIF. |
| Png | `262` | Portable Network Graphics. |
| Gif | `322` | Gif |
| WebP | `323` | Webp |
| Json | `513` | Json |
| SqlScript | `514` | SQL |
| Dbf | `515` | Archivo de datos Xbase |
| FlatOpc | `516` | Archivo opc plano. |
| XHtml | `771` | Representa un archivo XHtml. |
| OneNote | `772` | Representa un archivo One Note. |
| MicrosoftCabinet | `773` | Representa un archivo Microsoft Cabinet. |
| Rtf | `774` | Rtf |
| Epub | `775` | EPUB |
| Azw3 | `777` | AZW3 |
| Chm | `784` | CHM |
| Oxps | `776` | Formato OXPS (Open XML Paper Specification). |
| GZip | `35615` | Representa un archivo GZip. |
| Otg | `1025` | Representa un archivo OTG. |
| Odb | `1026` | Representa un archivo Odb. |
| Ofd | `1029` | Representa un archivo Ofd. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatTypeDemo
    {
        public static void FileFormatTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer el nombre de la hoja de cálculo
            worksheet.Name = "File Format Example";

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("File Format Type");
            worksheet.Cells["A2"].PutValue(FileFormatType.Csv);
            worksheet.Cells["A3"].PutValue(FileFormatType.Xlsx);
            worksheet.Cells["A4"].PutValue(FileFormatType.Pdf);
            worksheet.Cells["A5"].PutValue(FileFormatType.Xlsm);

            // Salida de los tipos de formato de archivo
            for (int i = 2; i <= 5; i++)
            {
                var fileFormat = worksheet.Cells[$"A{i}"].StringValue;
                Console.WriteLine($"Row {i}: {fileFormat}");
            }

            // Guarda el libro de trabajo
            workbook.Save("FileFormatTypeExample.xlsx");
            workbook.Save("FileFormatTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


