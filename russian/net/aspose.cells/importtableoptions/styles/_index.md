---
title: "ImportTableOptions.Styles"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImportTableOptions. Получает и задает стили для каждого столбца таблицы"
type: docs
url: /ru/net/aspose.cells/importtableoptions/styles/
---
## ImportTableOptions.Styles property

Получает и задаёт стили для каждого столбца таблицы.

```csharp
public Style[] Styles { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsPropertyStylesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать пример таблицы данных
            DataTable dt = new DataTable();
            dt.Columns.Add("Product");
            dt.Columns.Add("Price");
            dt.Rows.Add("Apple", 1.50);
            dt.Rows.Add("Banana", 0.75);
            dt.Rows.Add("Orange", 1.20);

            try
            {
                // Создать ImportTableOptions и задать свойство Styles
                ImportTableOptions options = new ImportTableOptions();
                options.IsFieldNameShown = true;

                // Создайте стили для каждого столбца
                Style[] columnStyles = new Style[2];

                // Стиль для столбца Product (жирный, синий шрифт)
                Style productStyle = workbook.CreateStyle();
                productStyle.Font.IsBold = true;
                productStyle.Font.Color = System.Drawing.Color.Blue;
                columnStyles[0] = productStyle;

                // Стиль для столбца Price (формат валюты, зеленый шрифт)
                Style priceStyle = workbook.CreateStyle();
                priceStyle.Font.Color = System.Drawing.Color.Green;
                priceStyle.Number = 4; // Currency format
                columnStyles[1] = priceStyle;

                // Установите свойство Styles
                options.Styles = columnStyles;

                // Импортировать данные со стилями
                worksheet.Cells.ImportData(dt, 0, 0, options);

                // Отобразить применённые стили
                Console.WriteLine("Styles applied to columns:");
                Console.WriteLine($"Product column style: Bold={columnStyles[0].Font.IsBold}, Color={columnStyles[0].Font.Color.Name}");
                Console.WriteLine($"Price column style: NumberFormat={columnStyles[1].Number}, Color={columnStyles[1].Font.Color.Name}");

                // Сохраните книгу
                workbook.Save("StylesDemo.xlsx");
                Console.WriteLine("Workbook saved with styled data.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


