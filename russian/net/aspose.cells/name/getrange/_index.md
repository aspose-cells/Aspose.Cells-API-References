---
title: "Name.GetRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Name method. Получает диапазон, если это имя ссылается на диапазон"
type: docs
url: /ru/net/aspose.cells/name/getrange/
---
## GetRange() {#getrange}

Получает диапазон, если это имя ссылается на диапазон.

```csharp
public Range GetRange()
```

### Возвращаемое значение

Диапазон.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            
            // Создать именованный диапазон
            int index = workbook.Worksheets.Names.Add("MyRange");
            workbook.Worksheets.Names[index].RefersTo = "=Sheet1!A1:B3";
            Name namedRange = workbook.Worksheets.Names[index];
            
            // Продемонстрировать метод GetRange
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Named Range Address: " + range.Address);
            Console.WriteLine("Worksheet Name: " + range.Worksheet.Name);
            
            // Изменить диапазон
            foreach (Cell cell in range)
            {
                if (cell.Row == 0)
                {
                    cell.PutValue(cell.StringValue.ToUpper());
                }
            }
            
            // Сохраните книгу
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(bool) {#getrange_1}

Получает диапазон, если это имя ссылается на диапазон

```csharp
public Range GetRange(bool recalculate)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| пересчитать | Boolean | нужно ли пересчитать его, если это имя уже было вычислено до этого вызова. |

### Возвращаемое значение

Диапазон.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Заполнить примерными данными
            for (int i = 0; i < 4; i++)
            {
                cells[i, 1].PutValue(i); // Column B values: 0,1,2,3
            }

            // Создать именованный диапазон с формулой
            int nameIndex = wb.Worksheets.Names.Add("testname");
            Name name = wb.Worksheets.Names[nameIndex];
            name.RefersTo = "IFERROR(Sheet1!$B$2:$B$4,-1)";

            // Использовать именованный диапазон в формулах
            cells["C1"].Formula = "=testname";
            cells["D1"].Formula = "SUM(testname)";

            // Вычислить формулы
            wb.CalculateFormula();

            // Получить диапазон, используя GetRange(true)
            Aspose.Cells.Range namedRange = name.GetRange(true);
            Console.WriteLine($"Named range: FirstRow={namedRange.FirstRow}, FirstColumn={namedRange.FirstColumn}, " +
                $"RowCount={namedRange.RowCount}, ColumnCount={namedRange.ColumnCount}");

            // Создать диаграмму, используя именованный диапазон
            int chartIndex = sheet.Charts.Add(ChartType.Column, 10, 1, 20, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("testname", true);
            Console.WriteLine($"Chart data points count: {chart.NSeries[0].CountOfDataValues}");
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(int, int, int) {#getrange_2}

Получает диапазон, если это имя ссылается на диапазон. Если ссылка этого имени не абсолютна, диапазон может различаться для разных ячеек.

```csharp
public Range GetRange(int sheetIndex, int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | Int32 | Соответствующий индекс листа. |
| строка | Int32 | Соответствующий индекс строки. |
| column | Int32 | Соответствующий индекс столбца |

### Возвращаемое значение

Диапазон.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Dairy");
            
            // Создать именованный диапазон, используя правильную сигнатуру метода
            int index = workbook.Worksheets.Names.Add("SubCat");
            workbook.Worksheets.Names["SubCat"].RefersTo = "=" + worksheet.Name + "!A2:A4";
            
            // Получить диапазон, используя GetRange с параметрами строки, столбца и количества строк
            Aspose.Cells.Range range = workbook.Worksheets.Names["SubCat"].GetRange(0, 0, 3);
            
            // Отобразить ссылку на диапазон
            Console.WriteLine("Range refers to: " + range.RefersTo);
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


