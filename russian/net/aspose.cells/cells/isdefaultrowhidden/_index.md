---
title: "Cells.IsDefaultRowHidden"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Указывает, скрыта ли строка по умолчанию"
type: docs
url: /ru/net/aspose.cells/cells/isdefaultrowhidden/
---
## Cells.IsDefaultRowHidden property

Указывает, скрыта ли строка по умолчанию.

```csharp
public bool IsDefaultRowHidden { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHiddenDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить свойство скрытия строки по умолчанию
            worksheet.Cells.IsDefaultRowHidden = true;
            
            // Отобразить текущее значение IsDefaultRowHidden
            Console.WriteLine("IsDefaultRowHidden: " + worksheet.Cells.IsDefaultRowHidden);
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


