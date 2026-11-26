---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор LowCodeSaveOptionsProviderOfPlaceHolders. Создаёт экземпляр для предоставления параметров сохранения согласно указанным шаблонам"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders constructor

Создает экземпляр для предоставления параметров сохранения в соответствии с указанными шаблонами.

```csharp
public LowCodeSaveOptionsProviderOfPlaceHolders(string pathTemplate)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pathTemplate | String | Шаблон результирующего пути к файлу. |

### Примечания

Поддерживаемые плейсхолдеры в шаблоне пути к файлу: ${SheetIndex}: будет заменён индексом листа части ${SheetName}: будет заменён именем листа части ${SplitPartIndex}: будет заменён индексом части ${SheetIndexPrefix}: будет заменён на [`SheetIndexPrefix`](../sheetindexprefix/) ${SheetNamePrefix}: будет заменён на [`SheetNamePrefix`](../sheetnameprefix/) ${SplitPartPrefix}: будет заменён на [`SplitPartPrefix`](../splitpartprefix/)

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersMethodCtorWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Вызовите метод #ctor с параметром String
                string pathTemplate = "output_{sheet}_part_{part}.xlsx";
                var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

                // Установите некоторые свойства
                provider.SheetIndexOffset = 0;
                provider.SplitPartIndexOffset = 0;
                provider.SheetNamePrefix = "Sheet_";
                provider.SplitPartPrefix = "Part_";

                Console.WriteLine("LowCodeSaveOptionsProviderOfPlaceHolders created successfully with path template: " + pathTemplate);
                Console.WriteLine($"SheetNamePrefix: {provider.SheetNamePrefix}, SplitPartPrefix: {provider.SplitPartPrefix}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LowCodeSaveOptionsProviderOfPlaceHolders: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("LowCodeSaveOptionsProviderDemo.xlsx");
        }
    }
}
```

### См. также

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


