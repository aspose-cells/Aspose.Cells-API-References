---
title: "Класс LowCodeLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.LowCode.LowCodeLoadOptions. Параметры для загрузки файла шаблона"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodeloadoptions/
---
## LowCodeLoadOptions class

Параметры загрузки файла шаблона.

```csharp
public class LowCodeLoadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LowCodeLoadOptions](lowcodeloadoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [InputFile](../../aspose.cells.lowcode/lowcodeloadoptions/inputfile/) { get; set; } | Получает и задаёт файл (с путём, если необходимо) шаблона. |
| [InputStream](../../aspose.cells.lowcode/lowcodeloadoptions/inputstream/) { get; set; } | Получает и задаёт поток Stream шаблона. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            // Создайте примерный поток (в памяти для демонстрационных целей)
            using (MemoryStream stream = new MemoryStream())
            {
                // Создайте новую книгу и сохраните её в поток для демонстрации
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Save(stream, SaveFormat.Xlsx);

                // Сбросьте позицию потока
                stream.Position = 0;

                // Создайте и используйте LowCodeLoadOptions
                var loadOptions = new LowCodeLoadOptions()
                {
                    InputStream = stream
                };

                // Пример использования — обычно передаётся в метод обработки
                Console.WriteLine($"Loading with LowCode options from stream of length: {loadOptions.InputStream.Length}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


