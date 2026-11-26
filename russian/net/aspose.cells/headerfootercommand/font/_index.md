---
title: "HeaderFooterCommand.Font"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HeaderFooterCommand. Получает шрифт значения команды"
type: docs
url: /ru/net/aspose.cells/headerfootercommand/font/
---
## HeaderFooterCommand.Font property

Получает шрифт значения команды.

```csharp
public Font Font { get; }
```

### Примечания

Бесполезно для HeaderFooterCommandType.Picture.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HeaderFooterCommandPropertyFontDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к настройкам страницы для заголовка/нижнего колонтитула
            PageSetup pageSetup = worksheet.PageSetup;

            // Установить заголовок с текстом, который будет содержать HeaderFooterCommand
            pageSetup.SetHeader(0, "&\"Arial\"&12&BThis is a header");

            // Получить скрипт заголовка
            string headerScript = pageSetup.GetHeader(0);

            // Получить команды заголовка
            HeaderFooterCommand[] commands = pageSetup.GetCommands(headerScript);

            // Найти текстовую команду (предполагая, что это первая)
            if (commands.Length > 0 && commands[0].Type == HeaderFooterCommandType.Text)
            {
                HeaderFooterCommand textCommand = commands[0];
                
                // Получить доступ к свойству Font (только для чтения)
                Font font = textCommand.Font;
                
                // Отобразить текущие свойства шрифта
                Console.WriteLine("Current Font:");
                Console.WriteLine($"Name: {font.Name}");
                Console.WriteLine($"Size: {font.Size}");
                Console.WriteLine($"Bold: {font.IsBold}");
                Console.WriteLine($"Color: {font.Color}");

                // Поскольку Font доступен только для чтения, мы не можем присвоить новый объект Font,
                // но мы можем изменить свойства существующего шрифта
                font.Name = "Times New Roman";
                font.Size = 14;
                font.IsBold = false;
                font.Color = System.Drawing.Color.Blue;

                // Сохраните рабочую книгу, чтобы увидеть изменения
                workbook.Save("HeaderFooterFontDemo.xlsx");

                Console.WriteLine("\nModified Font:");
                Console.WriteLine($"Name: {font.Name}");
                Console.WriteLine($"Size: {font.Size}");
                Console.WriteLine($"Bold: {font.IsBold}");
                Console.WriteLine($"Color: {font.Color}");
            }
        }
    }
}
```

### См. также

* class [Font](../../font/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


