---
title: "VbaModule.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaModule. Получает и задает имя модуля"
type: docs
url: /ru/net/aspose.cells.vba/vbamodule/name/
---
## VbaModule.Name property

Получает и задает имя модуля.

```csharp
public string Name { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();

            // Добавьте лист и получите его VBA‑модуль
            Worksheet sheet = wb.Worksheets[0];
            int moduleIndex = wb.VbaProject.Modules.Add(sheet);
            VbaModule module = wb.VbaProject.Modules[moduleIndex];

            // Установите имя модуля
            module.Name = "Sheet1";

            // Добавьте простой VBA‑код в модуль
            string vbaCode = "Private Sub Worksheet_SelectionChange(ByVal Target As Range)\r\n" +
                             "    MsgBox \"Sheet name: \" & Me.Name\r\n" +
                             "End Sub\r\n";
            module.Codes = vbaCode;

            // Сохраните в поток памяти (для демонстрации)
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsm);
            }
        }
    }
}
```

### См. также

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


