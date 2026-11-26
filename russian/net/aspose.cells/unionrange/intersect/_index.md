---
title: "UnionRange.Intersect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод UnionRange. Находит пересечение с другим диапазоном"
type: docs
url: /ru/net/aspose.cells/unionrange/intersect/
---
## Intersect(string) {#intersect_2}

Пересекает другой диапазон.

```csharp
public UnionRange Intersect(string range)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазон | String | Диапазон. |

### Примечания

Если два объединённых диапазона не пересекаются, возвращает null.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodIntersectWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторыми образцовыми данными
            worksheet.Cells["A1"].PutValue("A1");
            worksheet.Cells["B1"].PutValue("B1");
            worksheet.Cells["A2"].PutValue("A2");
            worksheet.Cells["B2"].PutValue("B2");

            // Создайте UnionRange, охватывающий A1:B2
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            try
            {
                // Вызовите Intersect со строковым параметром, представляющим диапазон A1:A2
                UnionRange intersectionResult = unionRange.Intersect("A1:A2");

                // Отобразите информацию о пересечении
                Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
                Console.WriteLine($"First row: {intersectionResult.FirstRow}");
                Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
                Console.WriteLine($"Row count: {intersectionResult.RowCount}");
                Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");

                // Выделите область пересечения
                Style highlightStyle = workbook.CreateStyle();
                highlightStyle.BackgroundColor = System.Drawing.Color.LightGreen;
                intersectionResult.SetStyle(highlightStyle);

                Console.WriteLine("Intersect method executed successfully with parameter (String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Intersect method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("UnionRangeMethodIntersectWithStringDemo.xlsx");
        }
    }
}
```

### См. также

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Intersect(UnionRange) {#intersect_1}

Пересекает другой диапазон.

```csharp
public UnionRange Intersect(UnionRange unionRange)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| unionRange | UnionRange | Диапазон. |

### Примечания

Если два объединённых диапазона не пересекаются, возвращает null.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodIntersectWithUnionRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните ячейки некоторыми данными
            worksheet.Cells["A1"].PutValue("A1");
            worksheet.Cells["B1"].PutValue("B1");
            worksheet.Cells["C1"].PutValue("C1");
            worksheet.Cells["A2"].PutValue("A2");
            worksheet.Cells["B2"].PutValue("B2");
            worksheet.Cells["C2"].PutValue("C2");

            // Создайте два объединённых диапазона
            UnionRange range1 = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
            UnionRange range2 = worksheet.Cells.CreateRange("B1:C2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("B1:C2") });

            try
            {
                // Вызовите метод Intersect с параметром UnionRange
                UnionRange intersectionResult = range1.Intersect(range2);

                // Отобразите информацию о пересечении
                Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
                Console.WriteLine($"First row: {intersectionResult.FirstRow}");
                Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
                Console.WriteLine($"Row count: {intersectionResult.RowCount}");
                Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");

                // Выделите область пересечения
                Style highlightStyle = workbook.CreateStyle();
                highlightStyle.BackgroundColor = System.Drawing.Color.Yellow;
                intersectionResult.SetStyle(highlightStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Intersect method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("UnionRangeMethodIntersectWithUnionRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Intersect(Range[]) {#intersect}

Пересекает другой диапазон.

```csharp
public UnionRange Intersect(Range[] ranges)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазоны | Range[] | Диапазон. |

### Примечания

Если два объединённых диапазона не пересекаются, возвращает null.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodIntersectWithRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте пример данных в ячейках
            worksheet.Cells["A1"].PutValue("A1");
            worksheet.Cells["B1"].PutValue("B1");
            worksheet.Cells["A2"].PutValue("A2");
            worksheet.Cells["B2"].PutValue("B2");

            // Создайте диапазоны для пересечения
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B1");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A1:A2");
            Aspose.Cells.Range[] rangesToIntersect = new Aspose.Cells.Range[] { range1, range2 };

            // Получите объединённый диапазон листа
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            try
            {
                // Вызовите метод Intersect с параметром Range[]
                UnionRange intersectionResult = unionRange.Intersect(rangesToIntersect);

                // Отобразить информацию о результате пересечения
                Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
                Console.WriteLine($"First row: {intersectionResult.FirstRow}");
                Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
                Console.WriteLine($"Row count: {intersectionResult.RowCount}");
                Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");

                // Выделите область пересечения
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.Yellow;
                intersectionResult.SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Intersect method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("UnionRangeMethodIntersectWithRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


