---
title: "UnionRange.FirstColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство UnionRange. Возвращает индекс первой колонки диапазона"
type: docs
url: /ru/net/aspose.cells/unionrange/firstcolumn/
---
## UnionRange.FirstColumn property

Получает индекс первого столбца диапазона.

```csharp
public int FirstColumn { get; }
```

### Примечания

Действует только когда содержит один диапазон.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyFirstColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторыми данными
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");

            // Создайте объединённый диапазон
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C1");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A2:C2");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Отобразите свойство FirstColumn
            Console.WriteLine("First column index of the union range: " + unionRange.FirstColumn);

            // Продемонстрируйте использование FirstColumn в операциях
            Console.WriteLine("First column name: " + CellsHelper.ColumnIndexToName(unionRange.FirstColumn));

            // Примените форматирование к первой колонке объединённого диапазона
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range firstColumnRange = worksheet.Cells.CreateRange(
                unionRange.FirstRow, unionRange.FirstColumn,
                unionRange.RowCount, 1);
            firstColumnRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });

            // Сохранить результат
            workbook.Save("UnionRangePropertyFirstColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


