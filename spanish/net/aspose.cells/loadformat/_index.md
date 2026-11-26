---
title: "Enumeración LoadFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.LoadFormat enum. Representa el formato de archivo de carga"
type: docs
url: /es/net/aspose.cells/loadformat/
---
## LoadFormat enumeration

Representa el formato de archivo de carga.

```csharp
public enum LoadFormat
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Auto | `0` | Representa el reconocimiento del formato automáticamente. |
| Csv | `1` | Archivo de texto de valores separados por comas (CSV). |
| CSV | `1` | Archivo de texto de valores separados por comas (CSV). NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Csv. Esta propiedad será eliminada 6 meses después desde abril de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado. |
| Xlsx | `6` | Representa un libro de trabajo o plantilla Office Open XML spreadsheetML, con o sin macros. |
| Tsv | `11` | Archivo de texto de valores separados por tabulaciones (TSV). |
| TSV | `11` | Archivo de texto de valores separados por tabulaciones (TSV). NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Tsv. Esta propiedad será eliminada 6 meses después desde abril de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado. |
| TabDelimited | `11` | Representa un archivo de texto delimitado por tabulaciones, lo mismo que Tsv. |
| Html | `12` | Representa un archivo html. |
| MHtml | `13` | Representa un archivo mhtml. |
| Ods | `14` | Archivo Open Document Sheet (ODS). |
| ODS | `14` | Archivo Open Document Sheet (ODS). NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Ods. Esta propiedad será eliminada 6 meses después desde abril de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado. |
| Excel97To2003 | `5` | Representa un archivo Excel97-2003 xls. |
| SpreadsheetML | `15` | Representa un archivo Excel 2003 xml. |
| Xlsb | `16` | Representa un archivo xlsb. |
| Ots | `31` | Archivo Open Document Template Sheet (OTS). |
| Numbers | `56` | Representa un archivo numbers. |
| Fods | `59` | Representa el formato de archivo OpenDocument Flat XML Spreadsheet (.fods). |
| FODS | `59` | Representa el formato de archivo OpenDocument Flat XML Spreadsheet (.fods). NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Fods. Esta propiedad será eliminada 6 meses después desde abril de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado. |
| Sxc | `60` | Representa el formato de archivo StarOffice Calc Spreadsheet (.sxc). |
| SXC | `60` | Representa el formato de archivo StarOffice Calc Spreadsheet (.sxc). NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Sxc. Esta propiedad será eliminada 6 meses después desde abril de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado. |
| Xml | `51` | Representa un archivo xml simple. |
| Epub | `52` | Representa un archivo EPUB. |
| Azw3 | `53` | Representa un archivo AZW3. |
| Chm | `54` | Representa un archivo CHM. |
| Markdown | `55` | Representa un archivo Markdown. |
| Unknown | `255` | Representa un formato no reconocido, no se puede cargar. |
| Image | `254` | Imagen |
| Json | `513` | Json |
| Dif | `30` | Formato de Intercambio de Datos. |
| Dbf | `515` | Archivo de datos Xbase |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFormatDemo
    {
        public static void LoadFormatExample()
        {
            // Cargar un archivo Excel en diferentes formatos usando Aspose.Cells
            string[] filePaths = {
                "LoadFormatDemo_original.xlsx",
                "LoadFormatDemo_original.xls",
                "LoadFormatDemo_original.csv",
                "LoadFormatDemo_original.json"
            };

            foreach (var filePath in filePaths)
            {
                // Determinar el formato de carga basado en la extensión del archivo
                LoadFormat loadFormat = GetLoadFormat(filePath);

                // Crear LoadOptions con el LoadFormat determinado
                LoadOptions loadOptions = new LoadOptions(loadFormat);

                // Cargar el libro de trabajo con las opciones de carga especificadas
                Workbook workbook = new Workbook(filePath, loadOptions);

                // Realizar algunas operaciones en el libro de trabajo
                Console.WriteLine($"Loaded file: {filePath}");
                Console.WriteLine($"Number of sheets: {workbook.Worksheets.Count}");

                // Guardar el libro de trabajo en un archivo nuevo
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

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


