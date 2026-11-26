---
title: "HeaderFooterCommand.Text"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HeaderFooterCommand. Получает текст команды"
type: docs
url: /ru/net/aspose.cells/headerfootercommand/text/
---
## HeaderFooterCommand.Text property

Получает текст команды.

```csharp
public string Text { get; }
```

### Примечания

Допустимо только для HeaderFooterCommandType.Text.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class HeaderFooterCommandPropertyTextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить заголовок с текстовой командой
            worksheet.PageSetup.SetHeader(1, "&\"Arial\"&12&KFF0000Sample Text Header");
            
            // Получить команды заголовка
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(worksheet.PageSetup.GetHeader(1));
            
            // Отобразить информацию о текстовой команде
            foreach (HeaderFooterCommand cmd in commands)
            {
                if (cmd.Type == HeaderFooterCommandType.Text)
                {
                    Console.WriteLine("Text command found:");
                    Console.WriteLine("Text: " + cmd.Text);
                    Console.WriteLine("Font: " + cmd.Font);
                    Console.WriteLine("Color: " + ColorTranslator.ToHtml(cmd.Font.Color));
                }
            }
            
            // Сохраните книгу
            workbook.Save("HeaderFooterTextDemo.xlsx");
        }
    }
}
```

### См. также

* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


