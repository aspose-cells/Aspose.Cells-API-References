---
title: "DifSaveOptions.DifSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор DifSaveOptions. Создаёт параметры для сохранения файла DIF."
type: docs
url: /ru/net/aspose.cells/difsaveoptions/difsaveoptions/
---
## DifSaveOptions constructor

Создаёт параметры для сохранения файла DIF.

```csharp
public DifSaveOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DifSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            DifSaveOptions saveOptions = new DifSaveOptions()
            {
                ClearData = true,
                CreateDirectory = true,
                RefreshChartCache = true
            };

            workbook.Save("DifSaveOptionsOutput.dif", saveOptions);
        }
    }
}
```

### См. также

* class [DifSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


