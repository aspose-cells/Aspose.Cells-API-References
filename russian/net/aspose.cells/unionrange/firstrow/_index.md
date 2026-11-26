---
title: "UnionRange.FirstRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство UnionRange. Возвращает индекс первой строки диапазона"
type: docs
url: /ru/net/aspose.cells/unionrange/firstrow/
---
## UnionRange.FirstRow property

Получает индекс первой строки диапазона.

```csharp
public int FirstRow { get; }
```

### Примечания

Действует только когда содержит один диапазон.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyFirstRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить примерными данными
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Row {row}, Col {col}";
                }
            }

            // Создайте объединённый диапазон из A2:C5 и A7:C9
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A2:C5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A7:C9");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Отобразите свойство FirstRow
            Console.WriteLine("FirstRow of union range: " + unionRange.FirstRow);

            // Продемонстрируйте использование, выделив первую строку
            Style highlightStyle = workbook.CreateStyle();
            highlightStyle.Font.IsBold = true;
            highlightStyle.ForegroundColor = System.Drawing.Color.LightGreen;
            highlightStyle.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range firstRowRange = worksheet.Cells.CreateRange(
                unionRange.FirstRow,
                unionRange.FirstColumn,
                1,
                unionRange.ColumnCount);
            firstRowRange.ApplyStyle(highlightStyle, new StyleFlag { FontBold = true, CellShading = true });

            // Создайте другой диапазон и сравните значения FirstRow
            Aspose.Cells.Range singleRange = worksheet.Cells.CreateRange("D1:F5");
            Console.WriteLine("FirstRow of single range: " + singleRange.FirstRow);
            Console.WriteLine("Is union range starting after single range? " + 
                (unionRange.FirstRow > singleRange.FirstRow));

            // Сохраните книгу
            workbook.Save("UnionRangeFirstRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


