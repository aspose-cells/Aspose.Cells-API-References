---
title: "Row.CopySettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Row. Копирует настройки строки, такие как стиль, высота, видимость ... и т.д."
type: docs
url: /ru/net/aspose.cells/row/copysettings/
---
## Row.CopySettings method

Копирует настройки строки, такие как стиль, высота, видимость и т.д.

```csharp
public void CopySettings(Row source, bool checkStyle)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| источник | Row | исходная строка, чьи настройки будут скопированы в эту. |
| checkStyle | Boolean | определяет, проверять и собирать стиль. Действует и требуется только когда два объекта строки принадлежат разным книгам и стили этих книг различаются. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodCopySettingsWithRowBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте и стилизуйте исходную строку.
            Row sourceRow = worksheet.Cells.Rows[0];
            Style sourceStyle = workbook.CreateStyle();
            sourceStyle.BackgroundColor = Color.Blue;
            sourceRow.ApplyStyle(sourceStyle, new StyleFlag { All = true });
            sourceRow.Height = 25;
            sourceRow.IsHidden = false;

            // Создайте целевую строку.
            Row targetRow = worksheet.Cells.Rows[1];
            
            // Продемонстрируйте CopySettings с параметром copyStyle=true.
            targetRow.CopySettings(sourceRow, true);

            // Проверьте, что настройки были скопированы.
            Console.WriteLine($"Target row height: {targetRow.Height}");
            Console.WriteLine($"Target row is hidden: {targetRow.IsHidden}");

            workbook.Save("RowCopySettingsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


