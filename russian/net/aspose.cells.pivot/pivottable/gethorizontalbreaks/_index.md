---
title: "PivotTable.GetHorizontalBreaks"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Получает список индексов строк сводной таблицы, где находятся горизонтальные разрывы страниц"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/gethorizontalbreaks/
---
## PivotTable.GetHorizontalBreaks method

Получает список индексов строк сводной таблицы, где находятся горизонтальные разрывы страниц

```csharp
[Obsolete("Use ivotTable.GetHorizontalPageBreaks() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetHorizontalBreaks()
```

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotTable.GetHorizontalPageBreaks(). Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Collections;

    public class PivotTableMethodGetHorizontalBreaksDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Вычислить данные для заполнения сводной таблицы
            pivotTable.CalculateData();

            try
            {
                // Получить горизонтальные разрывы (разрывы страниц) для сводной таблицы
                ArrayList horizontalBreaks = pivotTable.GetHorizontalBreaks();
                
                Console.WriteLine("Horizontal breaks (row indices):");
                foreach (int rowIndex in horizontalBreaks)
                {
                    Console.WriteLine(rowIndex);
                }

                // Добавить разрыв страницы в строке 3 для демонстрации
                worksheet.HorizontalPageBreaks.Add("A3");
                
                // Получить обновлённые горизонтальные разрывы
                horizontalBreaks = pivotTable.GetHorizontalBreaks();
                Console.WriteLine("\nHorizontal breaks after adding page break:");
                foreach (int rowIndex in horizontalBreaks)
                {
                    Console.WriteLine(rowIndex);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetHorizontalBreaks method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("PivotTableGetHorizontalBreaksDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


