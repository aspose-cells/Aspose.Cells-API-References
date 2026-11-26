---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.GetSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LowCodeSaveOptionsProviderOfPlaceHolders. Получает параметры сохранения, из которых берутся настройки вывода для текущей разделённой части"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/getsaveoptions/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.GetSaveOptions method

Получает параметры сохранения, из которых берутся настройки вывода для текущей части разделения.

```csharp
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersMethodGetSaveOptionsWithSplitPartInfoDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте экземпляр SplitPartInfo
            // Поскольку у SplitPartInfo нет конструктора без параметров, а свойства только для чтения,
            // Нам понадобится получить экземпляр из другого места API или использовать null, если это разрешено
            // Для демонстрации мы передадим null (предполагая, что метод его принимает)
            SplitPartInfo splitPartInfo = null;

            // Создайте экземпляр LowCodeSaveOptionsProviderOfPlaceHolders
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output_{sheet}.xlsx")
            {
                SheetIndexOffset = 0,
                SplitPartIndexOffset = 0,
                BuildPathWithSheetAlways = false,
                BuildPathWithSplitPartAlways = false,
                SheetNamePrefix = "sheet_",
                SheetIndexPrefix = "sheet_",
                SplitPartPrefix = "part_",
                SaveOptionsTemplate = new LowCodeSaveOptions
                {
                    SaveFormat = SaveFormat.Xlsx
                }
            };

            try
            {
                // Вызовите метод GetSaveOptions с параметром SplitPartInfo
                var saveOptions = provider.GetSaveOptions(splitPartInfo);
                
                Console.WriteLine("GetSaveOptions method executed successfully with SplitPartInfo parameter");
                Console.WriteLine($"Output file: {saveOptions.OutputFile}");
                Console.WriteLine($"Save format: {saveOptions.SaveFormat}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSaveOptions method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("MethodGetSaveOptionsWithSplitPartInfoDemo.xlsx");
        }
    }
}
```

### См. также

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


