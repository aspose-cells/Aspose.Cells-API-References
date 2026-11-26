---
title: "CellsHelper.MergeFiles"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Объединяет несколько больших файлов xls в один файл xls."
type: docs
url: /ru/net/aspose.cells/cellshelper/mergefiles/
---
## CellsHelper.MergeFiles method

Объединяет несколько больших файлов xls в один файл xls.

```csharp
public static void MergeFiles(string[] files, string cachedFile, string destFile)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| файлы | String[] | Файлы. |
| cachedFile | String | Кешированный файл. |
| destFile | String | Файл назначения. |

### Примечания

Этот метод поддерживает только объединение данных, стилей и формул в новый файл. Кешированный файл используется для хранения временных данных.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsHelperMethodMergeFilesWithStringStringDemo
    {
        public static void Run()
        {
            // Создать временные файлы Excel для объединения
            string[] filesToMerge = new string[2];
            filesToMerge[0] = "File1.xlsx";
            filesToMerge[1] = "File2.xlsx";

            // Создать образцы рабочих книг
            Workbook workbook1 = new Workbook();
            workbook1.Worksheets[0].Cells["A1"].PutValue("File 1 Content");
            workbook1.Save(filesToMerge[0]);

            Workbook workbook2 = new Workbook();
            workbook2.Worksheets[0].Cells["A1"].PutValue("File 2 Content");
            workbook2.Save(filesToMerge[1]);

            string cachedFile = "CacheFile.tmp";
            string outputFile = "MergedOutput.xlsx";

            try
            {
                // Вызвать MergeFiles с параметрами String[], String, String
                CellsHelper.MergeFiles(filesToMerge, cachedFile, outputFile);

                Console.WriteLine("Files merged successfully. Output saved to: " + outputFile);

                // Проверить объединённый файл
                Workbook mergedWorkbook = new Workbook(outputFile);
                Console.WriteLine("Merged content:");
                Console.WriteLine(mergedWorkbook.Worksheets[0].Cells["A1"].StringValue);
                Console.WriteLine(mergedWorkbook.Worksheets[1].Cells["A1"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error merging files: {ex.Message}");
            }
            finally
            {
                // Очистите временные файлы
                if (File.Exists(filesToMerge[0])) File.Delete(filesToMerge[0]);
                if (File.Exists(filesToMerge[1])) File.Delete(filesToMerge[1]);
                if (File.Exists(cachedFile)) File.Delete(cachedFile);
            }
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


