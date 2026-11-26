---
title: "Перечисление HeaderFooterCommandType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.HeaderFooterCommandType enum. Представляет тип команды заголовка и нижнего колонтитула"
type: docs
url: /ru/net/aspose.cells/headerfootercommandtype/
---
## HeaderFooterCommandType enumeration

Представляет тип команды заголовка и нижнего колонтитула.

```csharp
public enum HeaderFooterCommandType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Text | `0` | Текст. |
| CurrentPage | `1` | Текущий номер страницы |
| Pagecount | `2` | Количество страниц |
| CurrentDate | `3` | Текущая дата |
| CurrentTime | `4` | Текущее время |
| SheetName | `5` | Имя листа |
| FileName | `6` | Имя файла без пути |
| FilePath | `7` | Путь к файлу без имени файла |
| Picture | `8` | Изображение |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHeaderFooterCommandTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Установить заголовок с различными типами команд
                worksheet.PageSetup.SetHeader(0, "&[Page] of &[Pages] - &[Date] - &[Time] - &[File]");

                // Получить команды заголовка
                string headerScript = worksheet.PageSetup.GetHeader(0);
                HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(headerScript);

                // Продемонстрировать различные значения HeaderFooterCommandType
                foreach (HeaderFooterCommand cmd in commands)
                {
                    Console.WriteLine($"Command Type: {cmd.Type}");

                    // Проверить конкретные типы команд
                    if (cmd.Type == HeaderFooterCommandType.CurrentPage)
                    {
                        Console.WriteLine("Found CurrentPage command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.Pagecount)
                    {
                        Console.WriteLine("Found Pagecount command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.CurrentDate)
                    {
                        Console.WriteLine("Found CurrentDate command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.CurrentTime)
                    {
                        Console.WriteLine("Found CurrentTime command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.FileName)
                    {
                        Console.WriteLine("Found FileName command");
                    }
                }

                // Сохранить книгу, чтобы продемонстрировать настройку заголовка
                workbook.Save("HeaderFooterCommandTypeDemo.xlsx");
                Console.WriteLine("HeaderFooterCommandType demonstration completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HeaderFooterCommandType: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


