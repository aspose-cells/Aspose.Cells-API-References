---
title: "HyperlinkCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HyperlinkCollection. Получает элемент Hyperlink по указанному индексу"
type: docs
url: /ru/net/aspose.cells/hyperlinkcollection/item/
---
## HyperlinkCollection indexer

Получает элемент [`Hyperlink`](../../hyperlink/) по указанному индексу.

```csharp
public Hyperlink this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте гиперссылку в ячейку A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.example.com");
            
            // Получите первую гиперссылку с помощью свойства Item и задайте отображаемый текст
            worksheet.Hyperlinks[0].TextToDisplay = "Click Here";
            
            // Установить стиль гиперссылки (синий подчеркнутый текст)
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.Underline = FontUnderlineType.Single;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### См. также

* class [Hyperlink](../../hyperlink/)
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


