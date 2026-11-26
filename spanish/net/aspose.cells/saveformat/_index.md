---
title: "Enumeración SaveFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.SaveFormat. Representa el formato en el que se guarda el libro de trabajo"
type: docs
url: /es/net/aspose.cells/saveformat/
---
## SaveFormat enumeration

Representa el formato en el que se guarda el libro.

```csharp
public enum SaveFormat
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Csv | `1` | Archivo de texto de valores separados por comas (CSV). |
| CSV | `1` | Archivo de texto de valores separados por comas (CSV). NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Csv. Esta propiedad será eliminada 6 meses después desde abril de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado. |
| Xlsx | `6` | Representa un archivo xlsx. |
| Xlsm | `7` | Representa un archivo xlsm que permite macros. |
| Xltx | `8` | Representa un archivo xltx. |
| Xltm | `9` | Representa un archivo xltm que permite macros. |
| Xlam | `10` | Representa un archivo xltm que permite macros de complemento. |
| Tsv | `11` | Archivo de texto de valores separados por tabulaciones (TSV). |
| TSV | `11` | Archivo de texto de valores separados por tabulaciones (TSV). NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Tsv. Esta propiedad será eliminada 6 meses después desde abril de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado. |
| TabDelimited | `11` | Representa un archivo de texto delimitado por tabulaciones, lo mismo que Tsv. |
| Html | `12` | Representa un archivo html. |
| MHtml | `17` | Representa un archivo mhtml. |
| Ods | `14` | Archivo Open Document Sheet (ODS). |
| ODS | `14` | Archivo Open Document Sheet (ODS). NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Ods. Esta propiedad será eliminada 6 meses después desde abril de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado. |
| Excel97To2003 | `5` | Representa un archivo Excel97-2003 xls. |
| SpreadsheetML | `15` | Representa un archivo Excel 2003 xml. |
| Xlsb | `16` | Representa un archivo xlsb. |
| Auto | `0` | Si se guarda el archivo en el disco, el formato del archivo se ajusta a la extensión del nombre del archivo. Si se guarda el archivo en el flujo, el formato del archivo es xlsx. |
| Unknown | `255` | Representa un formato no reconocido, no se puede guardar. |
| Pdf | `13` | Representa un archivo PDF. |
| Xps | `20` | Formato XPS (XML Paper Specification). |
| XPS | `20` | Formato XPS (XML Paper Specification). NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Xps. Esta propiedad será eliminada 6 meses después de abril de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado. |
| Tiff | `21` | Representa un archivo TIFF. |
| TIFF | `21` | Representa un archivo TIFF. NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Tiff. Esta propiedad será eliminada 6 meses después de abril de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado. |
| Svg | `28` | Archivo SVG. |
| SVG | `28` | Archivo SVG. NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Svg. Esta propiedad será eliminada 6 meses después de abril de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado. |
| Dif | `30` | Formato de Intercambio de Datos. |
| Ots | `31` | Archivo Open Document Template Sheet (OTS). |
| Xlt | `32` | Archivo de plantilla Excel 97-2003. |
| Xml | `51` | Representa un archivo xml simple. |
| Numbers | `56` | Representa un archivo Numbers desde 2014 de Apple Inc. |
| Markdown | `57` | Representa un documento markdown. |
| Fods | `59` | Representa el formato de archivo OpenDocument Flat XML Spreadsheet (.fods). |
| FODS | `59` | Representa el formato de archivo OpenDocument Flat XML Spreadsheet (.fods). NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Fods. Esta propiedad será eliminada 6 meses después desde abril de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado. |
| Sxc | `60` | Representa el formato de archivo StarOffice Calc Spreadsheet (.sxc). |
| SXC | `60` | Representa el formato de archivo StarOffice Calc Spreadsheet (.sxc). NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Sxc. Esta propiedad será eliminada 6 meses después desde abril de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado. |
| Pptx | `61` | Representa un archivo .pptx. |
| Docx | `62` | Representa un archivo .docx. |
| Emf | `258` | Metarchivo mejorado de Windows. |
| Jpg | `261` | JPEG JFIF. |
| Png | `262` | Portable Network Graphics. |
| Bmp | `263` | Mapa de bits de Windows |
| Gif | `322` | Gif |
| Json | `513` | Json |
| SqlScript | `514` | SQL |
| XHtml | `771` | Representa un archivo XHtml. Por favor use la propiedad [`HtmlVersion`](../htmlsaveoptions/htmlversion/) . Esta propiedad será eliminada dentro de 6 meses a partir de marzo de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado. |
| Epub | `772` | Representa un archivo Epub. |
| Azw3 | `773` | Representa un archivo Azw3. |
| Pcl | `1025` | PCL (Lenguaje de Comando de Impresora) |
| Ofd | `1026` | OFD (Documento de diseño fijo abierto) |
| Dbf | `515` | Archivo de datos Xbase |

### Ejemplos

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class SaveFormatDemo
    {
        public static void SaveFormatExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Guarde el libro de trabajo en diferentes formatos
            workbook.Save("SaveFormatExample.xlsx", SaveFormat.Xlsx);
            workbook.Save("SaveFormatExample.xls", SaveFormat.Excel97To2003);
            workbook.Save("SaveFormatExample.csv", SaveFormat.Csv);
            workbook.Save("SaveFormatExample.pdf", SaveFormat.Pdf);
            workbook.Save("SaveFormatExample.html", SaveFormat.Html);

            // Genere la salida de los resultados
            Console.WriteLine("Workbook saved in multiple formats.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


