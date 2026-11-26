---
title: "FontSetting.FontSetting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор FontSetting."
type: docs
url: /ru/net/aspose.cells/fontsetting/fontsetting/
---
## FontSetting constructor

```csharp
public FontSetting(int startIndex, int length, WorksheetCollection sheets)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | Int32 |  |
| длина | Int32 |  |
| листы | WorksheetCollection |  |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingMethodCtorWithInt32Int32WorksheetCollectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить образец текста в ячейку
            worksheet.Cells["A1"].PutValue("Hello World");
            
            // Создать настройку шрифта для первых 5 символов (0-4) во всех листах
            FontSetting fontSetting = new FontSetting(0, 5, workbook.Worksheets);
            
            // Применить форматирование
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Size = 14;
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [WorksheetCollection](../../worksheetcollection/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


