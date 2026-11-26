---
title: "FindOptions.CaseSensitive"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FindOptions. Указывает, чувствителен ли регистр искомой строки"
type: docs
url: /ru/net/aspose.cells/findoptions/casesensitive/
---
## FindOptions.CaseSensitive property

Указывает, чувствителен ли искомый строк к регистру.

```csharp
public bool CaseSensitive { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить примерные данные
            worksheet.Cells["A1"].PutValue("ABC");
            worksheet.Cells["A2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("BcD");

            FindOptions options = new FindOptions();
            options.CaseSensitive = true;
            
            // Поиск "bc" с учётом регистра
            Cell cell = worksheet.Cells.Find("bc", null, options);
            
            Console.WriteLine(cell == null ? "Not found (case sensitive)" : $"Found at: {cell.Name}");
            
            options.CaseSensitive = false;
            cell = worksheet.Cells.Find("bc", null, options);
            
            Console.WriteLine(cell == null ? "Not found" : $"Found at: {cell.Name}");
        }
    }
}
```

### См. также

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


