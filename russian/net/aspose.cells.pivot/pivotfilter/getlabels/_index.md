---
title: "PivotFilter.GetLabels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotFilter. Получает метки фильтра заголовка"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfilter/getlabels/
---
## PivotFilter.GetLabels method

Получает метки фильтра подписи.

```csharp
public string[] GetLabels()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterMethodGetLabelsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создать корректную структуру сводной таблицы
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "A";
                worksheet.Cells["A3"].Value = "B";
                worksheet.Cells["A4"].Value = "A";
                
                // Создайте сводную таблицу с правильными параметрами
                int pivotIndex = worksheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // Создать сводный фильтр с корректными параметрами
                int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
                PivotFilter pivotFilter = pivotTable.PivotFilters[filterIndex];

                // Настроить свойства фильтра
                pivotFilter.Name = "SampleFilter";
                pivotFilter.EvaluationOrder = 1;

                // Выполнить метод GetLabels
                string[] labels = pivotFilter.GetLabels();

                Console.WriteLine($"Retrieved {labels?.Length ?? 0} labels:");
                if (labels != null)
                {
                    foreach (string label in labels)
                    {
                        Console.WriteLine($"- {label}");
                    }
                }

                workbook.Save("GetLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLabels: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


