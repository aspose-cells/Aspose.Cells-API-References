---
title: "CellArea.EndColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellArea alanı. Bu alanın son sütununu alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/cellarea/endcolumn/
---
## CellArea.EndColumn field

Bu alanın son sütununu alır veya ayarlar.

```csharp
public int EndColumn;
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // A1'den C3'e kadar bir hücre alanı oluşturun
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 2;

            // EndColumn kullanarak hücre alanını işleyin
            ProcessCellArea(area, Color.LightBlue, sheet);

            // Çalışma kitabını kaydedin
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

### Ayrıca Bakınız

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


