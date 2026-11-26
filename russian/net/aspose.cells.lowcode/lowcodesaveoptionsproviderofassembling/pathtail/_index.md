---
title: "LowCodeSaveOptionsProviderOfAssembling.PathTail"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSaveOptionsProviderOfAssembling. Добавляемая часть после номеров последовательности в пути к файлу. Должна включать расширение имени файла."
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathtail/
---
## LowCodeSaveOptionsProviderOfAssembling.PathTail property

Конечная часть (после последовательных номеров) пути файла. Она должна включать расширение имени файла.

```csharp
public string PathTail { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyPathTailDemo
    {
        public static void Run()
        {
            // Создать книгу с образцовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 25; i++)
            {
                worksheet.Cells[i, 0].Value = $"Record {i + 1}";
            }

            // Инициализировать провайдер параметров сохранения
            var optionsProvider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SalesReports/Q3",
                PathTail = ".xlsx",
                UseSheetName = true,
                SaveOptionsTemplate = new LowCodeSaveOptions
                {
                    SaveFormat = SaveFormat.Xlsx
                }
            };

            Console.WriteLine($"Original file extension: {optionsProvider.PathTail}");

            // Первое сохранение с расширением по умолчанию
            workbook.Save("output_original", optionsProvider.SaveOptionsTemplate.SaveFormat);

            // Измените хвост пути для вывода CSV
            optionsProvider.PathTail = "_split.csv";
            optionsProvider.SaveOptionsTemplate.SaveFormat = SaveFormat.Csv;
            Console.WriteLine($"Modified file extension: {optionsProvider.PathTail}");

            // Второе сохранение с новым расширением
            workbook.Save("output_modified", optionsProvider.SaveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check output directories for generated file formats");
        }
    }
}
```

### См. также

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


