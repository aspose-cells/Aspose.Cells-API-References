---
title: "Row.IsHeightMatched"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Row. Указывает, соответствует ли высота строки текущей настройке шрифта по умолчанию в книге. Значение true этого свойства также означает, что высота строки автоматическая без пользовательского значения высоты."
type: docs
url: /ru/net/aspose.cells/row/isheightmatched/
---
## Row.IsHeightMatched property

Указывает, соответствует ли высота строки текущим настройкам шрифта по умолчанию в рабочей книге. Значение true этого свойства также означает, что высота строки "автоматическая" без пользовательского значения высоты.

```csharp
public bool IsHeightMatched { get; set; }
```

### Примечания

Когда это свойство имеет значение true, если содержимое этой строки меняется, обычно высоту строки необходимо пересчитать (например, с помощью [`AutoFitRows`](../../worksheet/autofitrows/)), чтобы получить тот же результат, который отображается в MS Excel при открытии книги.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsHeightMatchedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите примерные данные и стиль, чтобы продемонстрировать соответствие высоты строки.
            worksheet.Cells["A1"].PutValue("This is a test string to demonstrate row height matching");
            worksheet.Cells["B1"].PutValue("Another cell in the same row");
            
            // Примените перенос слов, чтобы принудительно изменить высоту.
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Автоматически подгоните строку под высоту содержимого.
            worksheet.AutoFitRow(0);
            
            // Проверьте, соответствует ли высота строки её содержимому.
            Console.WriteLine("Is row height matched: " + worksheet.Cells.Rows[0].IsHeightMatched);
        }
    }
}
```

### См. также

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


