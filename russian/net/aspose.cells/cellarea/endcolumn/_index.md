---
title: "CellArea.EndColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Поле CellArea. Получает или задает конечный столбец этой области"
type: docs
url: /ru/net/aspose.cells/cellarea/endcolumn/
---
## CellArea.EndColumn field

Получает или задаёт конечный столбец этой области.

```csharp
public int EndColumn;
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellAreaFieldEndColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создайте область ячеек от A1 до C3
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 2;

            // Обработайте область ячеек, используя EndColumn
            ProcessCellArea(area, Color.LightBlue, sheet);

            // Сохраните книгу
            workbook.Save("CellAreaFieldEndColumnDemo_output.xlsx");
        }

        private static void ProcessCellArea(CellArea area, Color color, Worksheet sheet)
        {
            int k = 0;
            for (int col = area.StartColumn; col <= area.EndColumn; col++)
            {
                for (int row = area.StartRow; row <= area.EndRow; row++)
                {
                    Cell cell = sheet.Cells[row, col];
                    
                    if (!color.IsEmpty)
                    {
                        Style style = cell.GetStyle();
                        style.ForegroundColor = color;
                        style.Pattern = BackgroundType.Solid;
                        cell.SetStyle(style);
                    }
                    
                    cell.PutValue(row + col + k);
                    k++;
                }
            }
        }
    }
}
```

### См. также

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


