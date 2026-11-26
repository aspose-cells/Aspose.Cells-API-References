---
title: "Cells.GetMergedAreas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает все объединённые ячейки"
type: docs
url: /ru/net/aspose.cells/cells/getmergedareas/
---
## Cells.GetMergedAreas method

Получает все объединённые ячейки.

```csharp
public CellArea[] GetMergedAreas()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMergedAreasDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать несколько объединённых ячеек
            worksheet.Cells.Merge(0, 0, 2, 2); // Merge A1:B2
            worksheet.Cells.Merge(3, 3, 3, 2); // Merge D4:E4
            worksheet.Cells.Merge(5, 0, 1, 5); // Merge A6:E6
            
            // Получить все объединённые области
            CellArea[] mergedAreas = worksheet.Cells.GetMergedAreas();
            
            // Отобразить информацию об объединённых областях
            Console.WriteLine("Number of merged areas: " + mergedAreas.Length);
            foreach (CellArea area in mergedAreas)
            {
                Console.WriteLine($"Merged area: StartRow={area.StartRow}, StartColumn={area.StartColumn}, " +
                    $"EndRow={area.EndRow}, EndColumn={area.EndColumn}");
            }
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


