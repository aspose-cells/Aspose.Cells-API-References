---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSaveOptionsProviderOfPlaceHolders. Префикс для индекса листа"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix property

Префикс для индекса листа.

```csharp
public string SheetNamePrefix { get; set; }
```

### Примечания

Если существует только один лист и [`BuildPathWithSheetAlways`](../buildpathwithsheetalways/) равно false, то этот префикс и индекс листа (или его имя) не будут добавлены к результирующему пути файла.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetNamePrefixDemo
    {
        public static void Run()
        {
            // Создать новую книгу с двумя листами
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "SalesData";
            workbook.Worksheets.Add("FinancialReport");

            // Инициализируйте провайдер с шаблоном пути, содержащим заполнитель листа
            string pathTemplate = "output_{sheet}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Отобразите начальное значение SheetNamePrefix (по умолчанию пусто)
            Console.WriteLine("Initial SheetNamePrefix: " + provider.SheetNamePrefix);

            // Установите новый префикс и убедитесь, что генерация пути включает информацию о листе
            provider.SheetNamePrefix = "Q4_";
            provider.BuildPathWithSheetAlways = true;

            // Настройте параметры сохранения с правильным форматом
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx // Set the correct save format
            };

            // Сохраните книгу с помощью провайдера — генерируются "output_Q4_SalesData.xlsx" и "output_Q4_FinancialReport.xlsx"
            workbook.Save("result_directory", SaveFormat.Xlsx); // Pass correct SaveFormat
        }
    }
}
```

### См. также

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


