---
title: "Класс LowCodePdfSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.LowCode.LowCodePdfSaveOptions. Параметры сохранения PDF в режиме низкого кода"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodepdfsaveoptions/
---
## LowCodePdfSaveOptions class

Параметры сохранения PDF в режиме low code.

```csharp
public class LowCodePdfSaveOptions : LowCodeSaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LowCodePdfSaveOptions](lowcodepdfsaveoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Получает и задает файл (с путем, если необходимо) для сохранения сгенерированных данных. При установке этого свойства значением, отличным от null или пустой строки, [`OutputStream`](../lowcodesaveoptions/outputstream/) будет игнорироваться. (Унаследовано от [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Получает и задает поток для записи сгенерированных данных. При установке этого свойства значением, отличным от null, [`OutputFile`](../lowcodesaveoptions/outputfile/) будет игнорироваться. (Унаследовано от [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [PdfOptions](../../aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/) { get; set; } | Параметры сохранения PDF-файла. |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodepdfsaveoptions/saveformat/) { get; set; } | Формат сохранения для вывода. При конвертации в PDF он может быть только PDF. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodePdfSaveOptionsDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Создайте параметры сохранения PDF
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Compliance = PdfCompliance.PdfA1b;

            // Создать параметры сохранения PDF в режиме низкого кода
            LowCodePdfSaveOptions lowCodePdfOptions = new LowCodePdfSaveOptions()
            {
                OutputFile = "output.pdf",
                PdfOptions = pdfOptions
            };

            // Сохранить с помощью параметров низкого кода
            workbook.Save(lowCodePdfOptions.OutputFile, lowCodePdfOptions.PdfOptions);

            Console.WriteLine("File saved successfully with LowCodePdfSaveOptions");
        }
    }
}
```

### См. также

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


