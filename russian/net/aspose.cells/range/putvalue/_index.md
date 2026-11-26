---
title: "Range.PutValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Помещает значение в диапазон; при необходимости значение будет преобразовано к другому типу данных, а числовой формат ячеек будет сброшен"
type: docs
url: /ru/net/aspose.cells/range/putvalue/
---
## Range.PutValue method

Помещает значение в диапазон; при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stringValue | String | Входное значение |
| isConverted | Boolean | True: преобразовано в другой тип данных, если это уместно. |
| setStyle | Boolean | True: установить числовой формат в стиль ячейки при преобразовании в другой тип данных |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1:B10");
            range.PutValue("123", true, false);
            
            Console.WriteLine("Value at A5: " + cells["A5"].DoubleValue);
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


