---
title: "Workbook.MergeNamedStyles"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Объединяет именованные стили из другого файла Excel"
type: docs
url: /ru/net/aspose.cells/workbook/mergenamedstyles/
---
## Workbook.MergeNamedStyles method

Объединяет именованные стили из другого Excel-файла.

```csharp
public void MergeNamedStyles(Workbook source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| источник | Рабочая книга | Другой файл |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodMergeNamedStylesWithWorkbookDemo
    {
        public static void Run()
        {
            // Создайте целевую книгу (которая получит именованные стили)
            using (Workbook targetWorkbook = new Workbook())
            {
                // Добавьте некоторые данные в целевую книгу для контекста
                Worksheet targetSheet = targetWorkbook.Worksheets[0];
                targetSheet.Cells["A1"].PutValue("Target Workbook");

                // Создайте исходную книгу (которая содержит именованные стили для объединения)
                using (Workbook sourceWorkbook = new Workbook())
                {
                    // Добавьте некоторые данные в исходную книгу для контекста
                    Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
                    sourceSheet.Cells["A1"].PutValue("Source Workbook");

                    try
                    {
                        // Объедините именованные стили из sourceWorkbook в targetWorkbook
                        targetWorkbook.MergeNamedStyles(sourceWorkbook);

                        Console.WriteLine("MergeNamedStyles executed successfully.");

                        // Сохраните результирующую книгу
                        string outputPath = "MergedNamedStylesDemo.xlsx";
                        targetWorkbook.Save(outputPath, SaveFormat.Xlsx);
                        Console.WriteLine($"Workbook saved to '{outputPath}'.");
                    }
                    catch (Exception ex)
                    {
                        Console.WriteLine($"Error during MergeNamedStyles: {ex.Message}");
                    }
                }
            }
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


