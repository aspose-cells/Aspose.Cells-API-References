---
title: "StyleFlag.QuotePrefix"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройка Hide formula будет применена"
type: docs
url: /ru/net/aspose.cells/styleflag/quoteprefix/
---
## StyleFlag.QuotePrefix property

Настройка скрытия формулы будет применена.

```csharp
public bool QuotePrefix { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получите доступ к ячейке A1 и задайте значение, которое выглядит как число, но должно обрабатываться как текст
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("123456");

            // Создайте стиль и установите QuotePrefix в true
            Style style = workbook.CreateStyle();
            style.QuotePrefix = true;

            // Создайте флаг стиля и включите флаг QuotePrefix
            StyleFlag flag = new StyleFlag();
            flag.QuotePrefix = true;

            // Примените стиль к ячейке, используя SetStyle вместо ApplyStyle
            cell.SetStyle(style, flag);

            // Отобразите текущее значение QuotePrefix
            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);

            // Сохраните книгу, чтобы увидеть эффект (значение будет обрабатываться как текст в Excel)
            workbook.Save("PropertyQuotePrefixDemo.xlsx");

            // Теперь изменим QuotePrefix на false и посмотрим разницу
            style.QuotePrefix = false;
            cell.SetStyle(style, flag);

            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);
            // Сохраните снова под другим именем для сравнения
            workbook.Save("PropertyQuotePrefixDemo_WithoutPrefix.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


