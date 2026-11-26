---
title: "Cell.Characters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Возвращает объект Characters, представляющий диапазон символов внутри текста ячейки"
type: docs
url: /ru/net/aspose.cells/cell/characters/
---
## Cell.Characters method

Возвращает объект Characters, представляющий диапазон символов внутри текста ячейки.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | Int32 | Индекс начала символа. |
| длина | Int32 | Количество символов. |

### Возвращаемое значение

Объект Characters.

### Примечания

Этот метод работает только с ячейкой, содержащей строковое значение.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].PutValue("Helloworld");
            cells["A1"].Characters(5, 5).Font.IsBold = true;
            cells["A1"].Characters(5, 5).Font.Color = Color.Blue;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


