---
title: "UnionRange.Merge"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод UnionRange. Объединяет диапазон ячеек в одну ячейку"
type: docs
url: /ru/net/aspose.cells/unionrange/merge/
---
## UnionRange.Merge method

Объединяет диапазон ячеек в одну ячейку.

```csharp
public void Merge()
```

### Примечания

Ссылайтесь на объединённую ячейку через адрес верхней‑левой ячейки в диапазоне.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodMergeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте диапазон ячеек (A1:B2)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            
            // Поместите некоторые данные в ячейки, чтобы визуализировать объединение
            range[0, 0].PutValue("Before Merge");
            range[0, 1].PutValue("A1");
            range[1, 0].PutValue("B1");
            range[1, 1].PutValue("B2");
            
            try
            {
                // Создайте UnionRange из диапазона
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
                
                // Вызовите метод Merge
                unionRange.Merge();
                
                // Поместите значение в объединённую ячейку
                unionRange.PutValue("Merged A1:B2", true, true);
                
                Console.WriteLine("Cells merged successfully");
                
                // Раскомментируйте, чтобы увидеть эффект разъединения
                // unionRange.UnMerge();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Merge method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("MethodMergeDemo.xlsx");
        }
    }
}
```

### См. также

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


