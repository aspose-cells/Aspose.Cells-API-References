---
title: "CellRichValue.AltText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellRichValue. Возвращает альтернативный текст, связанный с изображением"
type: docs
url: /ru/net/aspose.cells/cellrichvalue/alttext/
---
## CellRichValue.AltText property

Получает альтернативный текст, связанный с изображением.

```csharp
public virtual string AltText { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellRichValuePropertyAltTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["C4"];
            
            cell.GetRichValue().AltText = "test alt text";
            
            Console.WriteLine("AltText: " + cell.GetRichValue().AltText);
        }
    }
}
```

### См. также

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


