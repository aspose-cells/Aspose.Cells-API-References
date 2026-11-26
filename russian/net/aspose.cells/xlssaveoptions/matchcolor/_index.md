---
title: "XlsSaveOptions.MatchColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XlsSaveOptions. Указывает, следует ли сопоставлять цвет шрифта, поскольку в стандартной палитре 56 цветов"
type: docs
url: /ru/net/aspose.cells/xlssaveoptions/matchcolor/
---
## XlsSaveOptions.MatchColor property

Указывает, следует ли сопоставлять цвет шрифта, поскольку в стандартной палитре 56 цветов.

```csharp
public bool MatchColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyMatchColorDemo
    {
        public static void Run()
        {
            // Создайте книгу и откройте первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получите доступ к ячейке B2 и задайте текст с определённым цветом шрифта
            Cell cellB2 = worksheet.Cells["B2"];
            cellB2.PutValue("Sample Text");
            
            // Установить цвет шрифта в синий
            Style style = cellB2.GetStyle();
            style.Font.Color = Color.Blue;
            cellB2.SetStyle(style);

            // Создать параметры сохранения с MatchColor, установленным в true
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MatchColor = true;

            // Сохраните книгу с указанными параметрами
            workbook.Save("output.xls", saveOptions);

            // Перезагрузить сохранённый файл, чтобы убедиться, что цвет сохранён
            Workbook savedWorkbook = new Workbook("output.xls");
            Cell savedCellB2 = savedWorkbook.Worksheets[0].Cells["B2"];
            
            // Проверить, что цвет шрифта всё ещё синий
            Color savedColor = savedCellB2.GetStyle().Font.Color;
            Console.WriteLine("Saved font color: " + savedColor.ToString());
        }
    }
}
```

### См. также

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


