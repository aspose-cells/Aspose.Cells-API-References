---
title: "LoadOptions.SetPaperSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LoadOptions. Устанавливает размер бумаги по умолчанию для печати из настроек принтеров по умолчанию"
type: docs
url: /ru/net/aspose.cells/loadoptions/setpapersize/
---
## LoadOptions.SetPaperSize method

Устанавливает размер бумаги по умолчанию из настроек принтера по умолчанию.

```csharp
public void SetPaperSize(PaperSizeType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | PaperSizeType | Размер бумаги по умолчанию. |

### Примечания

Если настройка размера бумаги отсутствует, MS Excel будет использовать настройки принтера по умолчанию.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsMethodSetPaperSizeWithPaperSizeTypeDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки и установить размер бумаги A5
            LoadOptions options = new LoadOptions();
            options.SetPaperSize(PaperSizeType.PaperA5);

            // Загрузить рабочую книгу с указанными параметрами
            Workbook workbook = new Workbook("example.xlsx", options);
            
            // Проверить, что размер бумаги установлен корректно
            Console.WriteLine("Paper size of first worksheet: " + workbook.Worksheets[0].PageSetup.PaperSize);
        }
    }
}
```

### См. также

* enum [PaperSizeType](../../papersizetype/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


