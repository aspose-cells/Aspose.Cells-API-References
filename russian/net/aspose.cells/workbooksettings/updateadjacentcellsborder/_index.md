---
title: "WorkbookSettings.UpdateAdjacentCellsBorder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Указывает, обновлять ли границы соседних ячеек"
type: docs
url: /ru/net/aspose.cells/workbooksettings/updateadjacentcellsborder/
---
## WorkbookSettings.UpdateAdjacentCellsBorder property

Указывает, следует ли обновлять границу соседних ячеек.

```csharp
public bool UpdateAdjacentCellsBorder { get; set; }
```

### Примечания

Значение по умолчанию — false. Например: нижняя граница ячейки A1 обновляется, верхняя граница ячейки A2 также должна быть изменена.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateAdjacentCellsBorderDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Включить обновление границ соседних ячеек
            workbook.Settings.UpdateAdjacentCellsBorder = true;

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить значение и применить границу к ячейке A1
            worksheet.Cells["A1"].PutValue("Sample");
            Style styleA1 = workbook.CreateStyle();
            styleA1.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            styleA1.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            worksheet.Cells["A1"].SetStyle(styleA1);

            // Установить значение в соседнюю ячейку B1 (справа от A1)
            worksheet.Cells["B1"].PutValue("Adjacent");

            // Сохраните книгу
            workbook.Save("output.xlsx");

            Console.WriteLine("Workbook saved with adjacent cell border update enabled.");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


