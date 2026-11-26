---
title: "Класс LowCodeSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.LowCode.LowCodeSaveOptions. Параметры сохранения сгенерированных результатов в режиме низкого кода"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptions/
---
## LowCodeSaveOptions class

Параметры сохранения сгенерированных результатов в режиме low code.

```csharp
public class LowCodeSaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LowCodeSaveOptions](lowcodesaveoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Получает и задает файл (с путем, если необходимо) для сохранения сгенерированных данных. При установке этого свойства значением, отличным от null или пустой строки, [`OutputStream`](./outputstream/) будет игнорироваться. |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Получает и задает поток для записи сгенерированных данных. При установке этого свойства значением, отличным от null, [`OutputFile`](./outputfile/) будет игнорироваться. |
| virtual [SaveFormat](../../aspose.cells.lowcode/lowcodesaveoptions/saveformat/) { get; set; } | Получает и задает формат сохранения для вывода. Обычно для конкретного процесса в режиме низкого кода разрешены только определённые форматы. Пожалуйста, укажите правильный формат для соответствующего процесса, иначе могут возникнуть неожиданные результаты или даже исключения. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeSaveOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте лист и внесите некоторые данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Создать параметры сохранения
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions()
            {
                OutputFile = "output.xlsx"
            };

            // Сохраните рабочую книгу, используя указанные параметры
            workbook.Save(saveOptions.OutputFile, saveOptions.SaveFormat);
            
            Console.WriteLine("File saved successfully with LowCodeSaveOptions");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


