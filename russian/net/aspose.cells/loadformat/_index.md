---
title: "Перечисление LoadFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.LoadFormat. Представляет формат загружаемого файла."
type: docs
url: /ru/net/aspose.cells/loadformat/
---
## LoadFormat enumeration

Представляет формат загружаемого файла.

```csharp
public enum LoadFormat
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Auto | `0` | Представляет автоматическое определение формата. |
| Csv | `1` | Текстовый файл значений, разделённых запятыми (CSV). |
| CSV | `1` | Текстовый файл значений, разделённых запятыми (CSV). ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Вместо него используйте свойство Csv. Это свойство будет удалено через 6 месяцев, начиная с апреля 2021 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать. |
| Xlsx | `6` | Представляет книгу или шаблон Office Open XML spreadsheetML, с макросами или без них. |
| Tsv | `11` | Текстовый файл значений, разделённых табуляцией (TSV). |
| TSV | `11` | Текстовый файл значений, разделённых табуляцией (TSV). ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Вместо него используйте свойство Tsv. Это свойство будет удалено через 6 месяцев, начиная с апреля 2021 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать. |
| TabDelimited | `11` | Представляет табуляционно-разделённый текстовый файл, аналогичный Tsv. |
| Html | `12` | Представляет HTML‑файл. |
| MHtml | `13` | Представляет MHTML‑файл. |
| Ods | `14` | Файл Open Document Sheet (ODS). |
| ODS | `14` | Файл Open Document Sheet (ODS). ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Вместо него используйте свойство Ods. Это свойство будет удалено через 6 месяцев, начиная с апреля 2021 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать. |
| Excel97To2003 | `5` | Представляет файл Excel97-2003 xls. |
| SpreadsheetML | `15` | Представляет файл Excel 2003 xml. |
| Xlsb | `16` | Представляет файл xlsb. |
| Ots | `31` | Файл Open Document Template Sheet (OTS). |
| Numbers | `56` | Представляет файл Numbers. |
| Fods | `59` | Представляет формат файла OpenDocument Flat XML Spreadsheet (.fods). |
| FODS | `59` | Представляет формат файла OpenDocument Flat XML Spreadsheet (.fods). ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Вместо него используйте свойство Fods. Это свойство будет удалено через 6 месяцев, начиная с апреля 2021 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать. |
| Sxc | `60` | Представляет формат файла StarOffice Calc Spreadsheet (.sxc). |
| SXC | `60` | Представляет формат файла StarOffice Calc Spreadsheet (.sxc). ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Вместо него используйте свойство Sxc. Это свойство будет удалено через 6 месяцев, начиная с апреля 2021 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать. |
| Xml | `51` | Представляет простой XML‑файл. |
| Epub | `52` | Представляет файл EPUB. |
| Azw3 | `53` | Представляет файл AZW3. |
| Chm | `54` | Представляет файл CHM. |
| Markdown | `55` | Представляет файл Markdown. |
| Unknown | `255` | Представляет нераспознанный формат, не может быть загружен. |
| Image | `254` | Изображение |
| Json | `513` | Json |
| Dif | `30` | Формат обмена данными. |
| Dbf | `515` | Файл данных Xbase |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFormatDemo
    {
        public static void LoadFormatExample()
        {
            // Загрузите файл Excel в разных форматах с помощью Aspose.Cells
            string[] filePaths = {
                "LoadFormatDemo_original.xlsx",
                "LoadFormatDemo_original.xls",
                "LoadFormatDemo_original.csv",
                "LoadFormatDemo_original.json"
            };

            foreach (var filePath in filePaths)
            {
                // Определите формат загрузки на основе расширения файла
                LoadFormat loadFormat = GetLoadFormat(filePath);

                // Создайте LoadOptions с определённым LoadFormat
                LoadOptions loadOptions = new LoadOptions(loadFormat);

                // Загрузите книгу с указанными параметрами загрузки
                Workbook workbook = new Workbook(filePath, loadOptions);

                // Выполните некоторые операции с книгой
                Console.WriteLine($"Loaded file: {filePath}");
                Console.WriteLine($"Number of sheets: {workbook.Worksheets.Count}");

                // Сохраните книгу в новый файл
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

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


