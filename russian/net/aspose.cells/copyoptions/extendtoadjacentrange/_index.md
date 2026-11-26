---
title: "CopyOptions.ExtendToAdjacentRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CopyOptions. Указывает, следует ли расширять диапазоны при копировании диапазона в соседний диапазон"
type: docs
url: /ru/net/aspose.cells/copyoptions/extendtoadjacentrange/
---
## CopyOptions.ExtendToAdjacentRange property

Указывает, расширять ли диапазоны при копировании диапазона в соседний диапазон.

```csharp
public bool ExtendToAdjacentRange { get; set; }
```

### Примечания

Если значение true, расширяется только диапазон гиперссылки, без добавления новой гиперссылки при копировании гиперссылок в соседние строки.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyExtendToAdjacentRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Добавьте гиперссылку в ячейку A1
            ws.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Создайте параметры копирования и установите ExtendToAdjacentRange в true
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ExtendToAdjacentRange = true;

            // Скопируйте строку 0 в строку 1 с параметрами копирования
            ws.Cells.CopyRows(ws.Cells, 0, 1, 1, copyOptions);

            // Проверьте, что гиперссылка была расширена до соседнего диапазона
            Console.WriteLine("Hyperlink count after copy: " + ws.Hyperlinks.Count);
        }
    }
}
```

### См. также

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


