---
title: "PageSetup.GetCommands"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Получает все команды заголовка или нижнего колонтитула"
type: docs
url: /ru/net/aspose.cells/pagesetup/getcommands/
---
## PageSetup.GetCommands method

Получает все команды верхнего или нижнего колонтитула.

```csharp
public HeaderFooterCommand[] GetCommands(string headerFooterScript)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| headerFooterScript | String | Скрипт заголовка/нижнего колонтитула |

### Возвращаемое значение

Возвращает все команды заголовка или нижнего колонтитула.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetCommandsWithStringDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить заголовок с командами
            string header = "&D&\"Arial\"&12sdfsdfsdfsdf";
            worksheet.PageSetup.SetHeader(1, header);
            
            // Получить команды заголовка
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(header);
            
            // Отобразить типы команд и текст
            foreach (HeaderFooterCommand cmd in commands)
            {
                Console.WriteLine($"Type: {cmd.Type}, Text: {cmd.Text}");
            }
        }
    }
}
```

### См. также

* class [HeaderFooterCommand](../../headerfootercommand/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


