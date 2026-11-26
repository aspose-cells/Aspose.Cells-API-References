---
title: "HeaderFooterCommand.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HeaderFooterCommand. Получает тип команды заголовка/нижнего колонтитула"
type: docs
url: /ru/net/aspose.cells/headerfootercommand/type/
---
## HeaderFooterCommand.Type property

Получает тип команды заголовка/нижнего колонтитула.

```csharp
public HeaderFooterCommandType Type { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HeaderFooterCommandPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить заголовок с различными типами команд
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(0, "&D&\"Arial\"&12sdfsdfsdfsdf");
            
            // Получить команды заголовка
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(0));
            
            // Продемонстрировать использование свойства Type
            Console.WriteLine("Command 0 Type: " + commands[0].Type); // CurrentDate
            Console.WriteLine("Command 1 Type: " + commands[1].Type); // Text
            Console.WriteLine("Command 1 Text: " + commands[1].Text); // sdfsdfsdfsdf
        }
    }
}
```

### См. также

* enum [HeaderFooterCommandType](../../headerfootercommandtype/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


