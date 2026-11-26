---
title: "Класс HeaderFooterCommand"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.HeaderFooterCommand. Представляет команду заголовка/нижнего колонтитула"
type: docs
url: /ru/net/aspose.cells/headerfootercommand/
---
## HeaderFooterCommand class

Представляет команду заголовка/нижнего колонтитула

```csharp
public class HeaderFooterCommand
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Font](../../aspose.cells/headerfootercommand/font/) { get; } | Получает шрифт значения команды. |
| [Text](../../aspose.cells/headerfootercommand/text/) { get; } | Получает текст команды. |
| [Type](../../aspose.cells/headerfootercommand/type/) { get; } | Получает тип команды заголовка/нижнего колонтитула. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHeaderFooterCommandDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получите доступ к PageSetup и задайте заголовок с помощью команд
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(1, "&D&\"Arial\"sdfsdfsdfsdf");
            
            // Получить команды заголовка
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(1));
            
            // Отобразить типы команд и текст
            Console.WriteLine("Command 1 Type: " + commands[0].Type);
            Console.WriteLine("Command 2 Type: " + commands[1].Type);
            Console.WriteLine("Command 2 Text: " + commands[1].Text);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


