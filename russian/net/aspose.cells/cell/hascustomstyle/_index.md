---
title: "Cell.HasCustomStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Указывает, имеет ли эта ячейка пользовательские настройки стиля, отличные от стиля по умолчанию, наследуемого от соответствующей строки, столбца или книги"
type: docs
url: /ru/net/aspose.cells/cell/hascustomstyle/
---
## Cell.HasCustomStyle property

Указывает, имеет ли эта ячейка пользовательские настройки стиля (отличные от стандартных, унаследованных от соответствующей строки, столбца или книги).

```csharp
public bool HasCustomStyle { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу и получить доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Check HasCustomStyle");

            // Отобразите начальное значение HasCustomState (наследует стиль по умолчанию)
            Console.WriteLine("Initial HasCustomStyle: " + cell.HasCustomStyle);

            // Создайте пользовательский стиль и примените его к ячейке
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.IsBold = true;
            cell.SetStyle(customStyle);

            // Проверьте, что HasCustomStyle равно true после изменения стиля
            Console.WriteLine("After applying custom style - HasCustomStyle: " + cell.HasCustomStyle);

            // Сохраните книгу с применённым пользовательским стилем
            workbook.Save("CellCustomStyleDemo.xlsx");

            // Сбросьте стиль ячейки к стилю по умолчанию книги
            Style defaultStyle = workbook.DefaultStyle;
            cell.SetStyle(defaultStyle);

            // Проверьте, что HasCustomStyle равно false после возврата к стилю по умолчанию
            Console.WriteLine("After resetting to default style - HasCustomStyle: " + cell.HasCustomStyle);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


