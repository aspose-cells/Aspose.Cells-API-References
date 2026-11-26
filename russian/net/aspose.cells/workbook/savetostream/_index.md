---
title: "Workbook.SaveToStream"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Сохраняет файл Excel в объект MemoryStream как файл Excel97-2003 xls и возвращает его"
type: docs
url: /ru/net/aspose.cells/workbook/savetostream/
---
## Workbook.SaveToStream method

Сохраняет файл Excel в объект MemoryStream как файл Excel97-2003 xls и возвращает его.

```csharp
public MemoryStream SaveToStream()
```

### Возвращаемое значение

Объект MemoryStream, содержащий файл xls Excel.

### Примечания

Этот метод предоставляет ту же функцию, что и метод Save, и сохраняет рабочую книгу только как файл Excel97-2003 xls. Он в основном предназначен для вызова из COM‑клиентов.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveToStreamDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook start = new Workbook();
            
            // Получите доступ к первому листу и добавьте некоторые примерные данные
            Worksheet worksheet = start.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Сохранить рабочую книгу в поток памяти
            MemoryStream stream = start.SaveToStream();

            // Создать новую рабочую книгу из потока
            Workbook workbook = new Workbook(stream);

            // Изменить новую рабочую книгу
            Worksheet newWorksheet = workbook.Worksheets[0];
            var area = CellArea.CreateCellArea(3, 0, 3, 1);
            newWorksheet.Cells.InsertRange(area, 3, ShiftType.Down, true);

            newWorksheet.Cells["A4"].PutValue("D");
            newWorksheet.Cells["B4"].PutValue(40);
            newWorksheet.Cells["A5"].PutValue("E");
            newWorksheet.Cells["B5"].PutValue(50);
            newWorksheet.Cells["A6"].PutValue("F");
            newWorksheet.Cells["B6"].PutValue(60);

            // Сохранить изменённую книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


