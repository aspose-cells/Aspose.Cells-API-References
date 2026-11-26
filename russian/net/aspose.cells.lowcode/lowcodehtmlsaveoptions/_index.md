---
title: "Класс LowCodeHtmlSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.LowCode.LowCodeHtmlSaveOptions класс. Параметры сохранения HTML в режиме low code"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/
---
## LowCodeHtmlSaveOptions class

Параметры сохранения HTML в режиме low code.

```csharp
public class LowCodeHtmlSaveOptions : LowCodeSaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LowCodeHtmlSaveOptions](lowcodehtmlsaveoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [HtmlOptions](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/) { get; set; } | Общие параметры сохранения HTML. |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Получает и задает файл (с путем, если необходимо) для сохранения сгенерированных данных. При установке этого свойства значением, отличным от null или пустой строки, [`OutputStream`](../lowcodesaveoptions/outputstream/) будет игнорироваться. (Унаследовано от [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Получает и задает поток для записи сгенерированных данных. При установке этого свойства значением, отличным от null, [`OutputFile`](../lowcodesaveoptions/outputfile/) будет игнорироваться. (Унаследовано от [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/saveformat/) { get; set; } | Получает и задаёт формат электронной таблицы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Widget");
            worksheet.Cells["B2"].PutValue(29.99);

            // Создать и настроить LowCodeHtmlSaveOptions
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                HtmlOptions = new HtmlSaveOptions()
                {
                    ExportWorksheetCSSSeparately = false,
                    ExportImagesAsBase64 = true
                }
            };

            // Сохранить рабочую книгу с настроенными HTML‑параметрами, используя параметр параметров сохранения
            workbook.Save("LowCodeHtmlExport.html", saveOptions.HtmlOptions);

            Console.WriteLine("HTML file saved successfully with low code options.");
        }
    }
}
```

### См. также

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


