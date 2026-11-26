---
title: "WorkbookRender.GetPageSizeInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorkbookRender. Получить размер страницы в дюймах выходного изображения"
type: docs
url: /ru/net/aspose.cells.rendering/workbookrender/getpagesizeinch/
---
## WorkbookRender.GetPageSizeInch method

Получить размер страницы в дюймах выходного изображения.

```csharp
public float[] GetPageSizeInch(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Индекс страницы начинается с нуля. |

### Возвращаемое значение

Размер изображения, [0] — ширина и [1] — высота

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test page size");
            sheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            WorkbookRender wr = new WorkbookRender(wb, imgOpt);
            
            float[] pageSize = wr.GetPageSizeInch(0);
            Console.WriteLine($"Page size in inches: {pageSize[0]} x {pageSize[1]}");
        }
    }
}
```

### См. также

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


