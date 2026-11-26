---
title: "UnionRange.UnMerge"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод UnionRange. Разъединяет объединённые ячейки этого диапазона"
type: docs
url: /ru/net/aspose.cells/unionrange/unmerge/
---
## UnionRange.UnMerge method

Разъединяет объединённые ячейки этого диапазона.

```csharp
public void UnMerge()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте диапазон и объедините ячейки
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
            
            // Объедините ячейки и задайте значение
            unionRange.Merge();
            unionRange.PutValue("Merged Cells", true, true);
            
            try
            {
                // Вызовите метод UnMerge
                unionRange.UnMerge();
                
                Console.WriteLine("Cells unmerged successfully");
                
                // Поместите значения в разъединённые ячейки, чтобы продемонстрировать эффект
                worksheet.Cells["A1"].PutValue("A1");
                worksheet.Cells["A2"].PutValue("A2");
                worksheet.Cells["B1"].PutValue("B1");
                worksheet.Cells["B2"].PutValue("B2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnMerge method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("MethodUnMergeDemo.xlsx");
        }
    }
}
```

### См. также

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


