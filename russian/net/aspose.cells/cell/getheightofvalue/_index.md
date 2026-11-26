---
title: "Cell.GetHeightOfValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получает высоту значения в пикселях"
type: docs
url: /ru/net/aspose.cells/cell/getheightofvalue/
---
## Cell.GetHeightOfValue method

Получает высоту значения в пикселях.

```csharp
public int GetHeightOfValue()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetHeightOfValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите значение и измерьте высоту
            worksheet.Cells["A1"].PutValue("Sample Text");
            double height = worksheet.Cells["A1"].GetHeightOfValue();
            
            Console.WriteLine("Height of value in A1: " + height);
            
            // Отрегулируйте высоту строки и измерьте снова
            worksheet.Cells.Rows[0].Height = 30;
            height = worksheet.Cells["A1"].GetHeightOfValue();
            
            Console.WriteLine("Height after row adjustment: " + height);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


