---
title: "DynamicFilter.MaxValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DynamicFilter. Получает и задает максимальное значение динамического фильтра"
type: docs
url: /ru/net/aspose.cells/dynamicfilter/maxvalue/
---
## DynamicFilter.MaxValue property

Получает и задает максимальное значение динамического фильтра.

```csharp
public object MaxValue { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyMaxValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить пример числовых данных
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);

            // Создать автофильтр
            worksheet.AutoFilter.Range = "A1:A6";
            
            // Применить динамический фильтр с критериями диапазона
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // Отобразить текущее MaxValue
            Console.WriteLine("Current MaxValue: " + filter.MaxValue);

            // Поскольку DynamicFilterType.Between не существует, мы будем использовать другой подход
            // Например, мы можем вместо этого использовать пользовательский фильтр
            worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterOrEqual, 20);
            worksheet.AutoFilter.Custom(0, FilterOperatorType.LessOrEqual, 40);

            // Применить фильтр
            worksheet.AutoFilter.Refresh();

            // Сохранить результат
            workbook.Save("DynamicFilterMaxValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


