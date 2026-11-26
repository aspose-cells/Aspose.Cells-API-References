---
title: "Cells.IsDefaultColumnHidden"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells."
type: docs
url: /ru/net/aspose.cells/cells/isdefaultcolumnhidden/
---
## Cells.IsDefaultColumnHidden property

```csharp
public bool IsDefaultColumnHidden { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultColumnHiddenDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте новую книгу и получите первый лист
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Добавьте некоторые данные, чтобы лист не был пустым
                cells["A1"].PutValue("First");
                cells["B1"].PutValue("Second");
                cells["C1"].PutValue("Third");

                // Прочитайте свойство IsDefaultColumnHidden (по умолчанию false)
                bool isDefaultColumnHidden = cells.IsDefaultColumnHidden;
                Console.WriteLine("IsDefaultColumnHidden: " + isDefaultColumnHidden);

                // Сохраните рабочую книгу (необязательно, только для завершения демонстрации)
                workbook.Save("IsDefaultColumnHiddenDemo.xlsx", SaveFormat.Xlsx);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


