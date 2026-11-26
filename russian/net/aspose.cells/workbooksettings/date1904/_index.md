---
title: "WorkbookSettings.Date1904"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает или задает значение, указывающее, использует ли книга систему дат 1904 года"
type: docs
url: /ru/net/aspose.cells/workbooksettings/date1904/
---
## WorkbookSettings.Date1904 property

Получает или задает значение, указывающее, использует ли рабочая книга систему дат 1904 года.

```csharp
public bool Date1904 { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDate1904Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Date1904 = true;

            Worksheet sheet = wb.Worksheets[0];
            Cell cell = sheet.Cells[0, 0];
            
            // Продемонстрировать отрицательное время с Date1904
            Style style = cell.GetStyle();
            style.Custom = "h:mm";
            cell.SetStyle(style);
            cell.PutValue(-0.0736111111111112);
            Console.WriteLine("Negative time value: " + cell.DisplayStringValue);

            // Продемонстрировать отрицательную дату с Date1904
            style = cell.GetStyle();
            style.Custom = "mm/dd/yyyy h:mm:ss";
            cell.SetStyle(style);
            cell.PutValue(-42389.47075706);
            Console.WriteLine("Negative date value: " + cell.DisplayStringValue);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


