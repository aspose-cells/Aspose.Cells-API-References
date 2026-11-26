---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexOffset"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSaveOptionsProviderOfPlaceHolders. Смещение индекса листов между тем, что используется в пути файла, и его фактическим значением SheetIndex"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexoffset/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexOffset property

Смещение индекса листа между тем, что используется в пути к файлу, и его фактическим значением ([`SheetIndex`](../../splitpartinfo/sheetindex/)).

```csharp
public int SheetIndexOffset { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetIndexOffsetDemo
    {
        public static void Run()
        {
            // Создайте новую книгу с несколькими листами.
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Создайте экземпляр LowCodeSaveOptionsProviderOfPlaceHolders
            string pathTemplate = "output_{sheet_index}.xlsx";
            var optionsProvider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Отобразите текущее значение SheetIndexOffset (по умолчанию 0)
            Console.WriteLine("Current SheetIndexOffset value: " + optionsProvider.SheetIndexOffset);

            // Установите SheetIndexOffset в 1, чтобы сдвинуть индексы листов в именах выходных файлов
            optionsProvider.SheetIndexOffset = 1;
            Console.WriteLine("New SheetIndexOffset value: " + optionsProvider.SheetIndexOffset);

            // Настроить параметры сохранения
            optionsProvider.SaveOptionsTemplate = new LowCodeSaveOptions();
            optionsProvider.SaveOptionsTemplate.SaveFormat = SaveFormat.Xlsx;

            // Продемонстрируйте влияние SheetIndexOffset на имена выходных файлов
            // Обычно это используется с GetSaveOptions() во время реальных операций сохранения
            Console.WriteLine("With SheetIndexOffset=1, output files would be named:");
            Console.WriteLine("Sheet1 -> output_1.xlsx (original index 0 + offset 1)");
            Console.WriteLine("Sheet2 -> output_2.xlsx (original index 1 + offset 1)");
            Console.WriteLine("Sheet3 -> output_3.xlsx (original index 2 + offset 1)");

            // Сбросить к значению по умолчанию
            optionsProvider.SheetIndexOffset = 0;
        }
    }
}
```

### См. также

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


