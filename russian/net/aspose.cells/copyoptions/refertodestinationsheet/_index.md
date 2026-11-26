---
title: "CopyOptions.ReferToDestinationSheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CopyOptions. При копировании диапазона в том же файле и когда диаграмма ссылается на исходный лист False означает, что источник данных скопированной диаграммы не будет изменён. True означает, что источник данных скопированной диаграммы будет ссылаться на лист назначения."
type: docs
url: /ru/net/aspose.cells/copyoptions/refertodestinationsheet/
---
## CopyOptions.ReferToDestinationSheet property

При копировании диапазона в том же файле, если диаграмма ссылается на исходный лист, значение False означает, что источник данных скопированной диаграммы не будет изменён. Значение True означает, что источник данных скопированной диаграммы будет ссылаться на лист назначения.

```csharp
public bool ReferToDestinationSheet { get; set; }
```

### Примечания

Значение по умолчанию — false, работает как в MS Excel. Например: при копировании диаграммы с источником данных "sheet1!A1:B10" из листа "sheet1" в другой лист "sheet2" источник данных будет изменён на "sheet2!A1:B10".

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToDestinationSheetDemo
    {
        public static void Run()
        {
            // Создайте исходную книгу с образцовыми данными
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B1"].PutValue(100);
            sourceSheet.Cells["A2"].PutValue("=SUM(B1)");

            // Создайте целевую книгу
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets.Add("DestinationSheet");

            // Установите параметры копирования с ReferToDestinationSheet
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ReferToDestinationSheet = true;

            // Скопируйте лист с указанными параметрами
            destSheet.Copy(sourceSheet, copyOptions);

            // Сохранить результат
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


