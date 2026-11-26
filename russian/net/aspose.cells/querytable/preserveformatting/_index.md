---
title: "QueryTable.PreserveFormatting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство QueryTable. Возвращает или задает PreserveFormatting объекта"
type: docs
url: /ru/net/aspose.cells/querytable/preserveformatting/
---
## QueryTable.PreserveFormatting property

Возвращает или задает PreserveFormatting объекта.

```csharp
public bool PreserveFormatting { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные и форматирование.
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Применить форматирование к диапазону данных
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // Применить стиль к каждой ячейке в диапазоне
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["B1"].SetStyle(style);

            // Создайте таблицу запросов (симулировано, так как реальное создание требует внешнего источника данных)
            // В реальном использовании вы бы создали это из внешнего соединения
            QueryTable queryTable = worksheet.QueryTables[0];

            // Отобразить текущее значение PreserveFormatting
            Console.WriteLine("Initial PreserveFormatting value: " + queryTable.PreserveFormatting);

            // Установить PreserveFormatting в false (не будет сохранять существующее форматирование при обновлении)
            queryTable.PreserveFormatting = false;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // Симулировать обновление таблицы запросов (обычно форматирование будет очищено, когда PreserveFormatting установлен в false)
            // В реальном сценарии это происходит, когда таблица запросов обновляет свои данные
            Console.WriteLine("After refresh with PreserveFormatting=false, formatting would be lost");

            // Установить PreserveFormatting обратно в true
            queryTable.PreserveFormatting = true;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // Симулировать повторное обновление (теперь будет сохраняться форматирование)
            Console.WriteLine("After refresh with PreserveFormatting=true, formatting is preserved");

            // Сохраните книгу
            workbook.Save("QueryTablePreserveFormattingDemo.xlsx");
        }
    }
}
```

### См. также

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


