---
title: "LowCodeSaveOptionsProviderOfAssembling.UseSheetName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSaveOptionsProviderOfAssembling. Определяет, формирует ли путь к файлу с именем листа вместо индекса листа. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/
---
## LowCodeSaveOptionsProviderOfAssembling.UseSheetName property

Создавать ли путь файла с именем листа вместо его индекса. Значение по умолчанию — false.

```csharp
public bool UseSheetName { get; set; }
```

### Примечания

Имя листа никогда не будет восстанавливаться автоматически. Поэтому, устанавливая его в true, убедитесь, что нет специального имени листа, которое может привести к недопустимому пути к файлу или имени.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyUseSheetNameDemo
    {
        public static void Run()
        {
            // Создайте новую книгу с именованным листом
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "MonthlyReport";
            
            // Добавьте примерные данные для демонстрации разбиения
            for(int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Record {i+1}");
            }

            // Создайте и настройте провайдер
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "split_files/",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet_",
                SplitPartPrefix = "Part_",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Продемонстрируйте UseSheetName=false (по умолчанию)
            Console.WriteLine($"Default UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_default", provider.SaveOptionsTemplate.SaveFormat);

            // Измените свойство и продемонстрируйте новое поведение
            provider.UseSheetName = true;
            Console.WriteLine($"\nModified UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_modified", provider.SaveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check 'split_files' directory for output files with different naming schemes");
        }
    }
}
```

### См. также

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


