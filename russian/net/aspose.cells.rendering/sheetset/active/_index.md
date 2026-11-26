---
title: "SheetSet.Active"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SheetSet. Возвращает набор с активным листом книги"
type: docs
url: /ru/net/aspose.cells.rendering/sheetset/active/
---
## SheetSet.Active property

Получает набор с активным листом книги.

```csharp
public static SheetSet Active { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyActiveDemo
    {
        public static void Run()
        {
            // Создать новую книгу с двумя листами
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Установите второй лист как активный
            workbook.Worksheets.ActiveSheetIndex = 1;

            // Добавьте данные в оба листа
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Active Sheet Data");

            // Создайте параметры сохранения PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Сохраните только активный лист
            pdfSaveOptions.SheetSet = SheetSet.Active;
            workbook.Save("ActiveSheetOnly.pdf", pdfSaveOptions);

            // Сохраните все листы для сравнения
            pdfSaveOptions.SheetSet = SheetSet.All;
            workbook.Save("AllSheets.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


