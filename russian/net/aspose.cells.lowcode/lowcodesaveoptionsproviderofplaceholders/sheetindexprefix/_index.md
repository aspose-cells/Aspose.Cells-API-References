---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSaveOptionsProviderOfPlaceHolders. Префикс для индекса листа"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix property

Префикс для индекса листа.

```csharp
public string SheetIndexPrefix { get; set; }
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

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetIndexPrefixDemo
    {
        public static void Run()
        {
            // Создать новую книгу с несколькими листами
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Создайте экземпляр LowCodeSaveOptionsProviderOfPlaceHolders
            string pathTemplate = "output_{sheetindex}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Отобразите и измените SheetIndexPrefix
            Console.WriteLine("Original SheetIndexPrefix: " + provider.SheetIndexPrefix);
            provider.SheetIndexPrefix = "sheet_";
            Console.WriteLine("Modified SheetIndexPrefix: " + provider.SheetIndexPrefix);

            // Установите другие необходимые свойства
            provider.BuildPathWithSheetAlways = true;
            provider.SaveOptionsTemplate = new LowCodeSaveOptions();

            // Продемонстрируйте влияние SheetIndexPrefix на пути к файлам
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                // Поскольку мы не можем создать и заполнить SplitPartInfo напрямую,
                // мы просто продемонстрируем шаблон именования без него
                Console.WriteLine($"Sheet {sheet.Name} would save to: output_{provider.SheetIndexPrefix}{sheet.Index}.xlsx");
            }

            // Сохраните книгу, чтобы продемонстрировать шаблон именования
            workbook.Save("output_sheet_0.xlsx");
        }
    }
}
```

### См. также

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


