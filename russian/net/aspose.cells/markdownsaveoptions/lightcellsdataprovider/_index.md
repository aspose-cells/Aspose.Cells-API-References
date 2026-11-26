---
title: "MarkdownSaveOptions.LightCellsDataProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MarkdownSaveOptions. Провайдер данных, предоставляющий данные ячеек для сохранения книги в легком режиме"
type: docs
url: /ru/net/aspose.cells/markdownsaveoptions/lightcellsdataprovider/
---
## MarkdownSaveOptions.LightCellsDataProvider property

Поставщик данных для предоставления данных ячеек при сохранении книги в облегчённом режиме.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections.Generic;

    public class MarkdownSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторыми образцовыми данными
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = "Item " + (i + 1);
                worksheet.Cells[i, 1].Value = i + 1;
            }

            // Создайте пользовательский LightCellsDataProvider
            var dataProvider = new CustomLightCellsDataProvider();

            // Создайте MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            
            // Отобразите текущее значение (по умолчанию должно быть null)
            Console.WriteLine("Current LightCellsDataProvider value: " + (saveOptions.LightCellsDataProvider == null ? "null" : "set"));

            // Установите пользовательский провайдер данных
            saveOptions.LightCellsDataProvider = dataProvider;

            // Сохраните с пользовательским провайдером данных
            workbook.Save("LightCellsDataProviderDemo.md", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private List<string> items = new List<string> { "Apple", "Banana", "Cherry", "Date", "Elderberry" };
        private List<double> values = new List<double> { 1.99, 0.99, 2.99, 3.49, 4.99 };
        private int currentRow = -1;

        public bool StartSheet(int sheetIndex)
        {
            // Обрабатывайте только первый лист
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            currentRow++;
            return currentRow < items.Count ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            // Установите высоту строки при необходимости
            row.Height = 15;
        }

        public int NextCell()
        {
            if (currentRow == -1)
            {
                // Заголовочная строка
                return currentRow < 2 ? currentRow + 1 : -1;
            }
            else
            {
                return currentRow < 2 ? currentRow + 1 : -1;
            }
        }

        public void StartCell(Cell cell)
        {
            if (currentRow == -1)
            {
                // Заголовок
                if (cell.Column == 0)
                    cell.Value = "Product";
                else if (cell.Column == 1)
                    cell.Value = "Price";
            }
            else
            {
                // Данные
                if (cell.Column == 0)
                    cell.Value = items[currentRow];
                else if (cell.Column == 1)
                    cell.Value = values[currentRow];
            }
        }

        public bool IsGatherString()
        {
            return false;
        }
    }
}
```

### См. также

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


