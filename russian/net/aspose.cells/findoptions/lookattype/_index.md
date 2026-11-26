---
title: "FindOptions.LookAtType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FindOptions. Тип просмотра"
type: docs
url: /ru/net/aspose.cells/findoptions/lookattype/
---
## FindOptions.LookAtType property

Посмотреть тип.

```csharp
public LookAtType LookAtType { get; set; }
```

### Примечания

Когда [`RegexKey`](../regexkey/) имеет значение true и пользователь указал точное правило для регулярного выражения, из соображений производительности это свойство следует установить в EntireContent. В противном случае мы будем рефакторить поисковый ключ, чтобы гарантировать его соответствие конкретному типу. Например, когда тип — Contains (это значение по умолчанию для этого свойства), мы автоматически добавим подстановочные символы в начало и конец поискового ключа. В этом случае регулярные выражения станут более сложными, и производительность также снизится.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookAtTypeDemo
    {
        public static void Run()
        {
            // Создайте книгу и добавьте некоторые данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("=1+2"); // Formula
            worksheet.Cells["A3"].PutValue("Partial match test");
            worksheet.Cells["A4"].PutValue("=A1&A3"); // Formula concatenating cells

            // Создайте параметры поиска с LookAtType.EntireContent
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.EntireContent
            };

            // Ищите формулу, точно соответствующую "=A1&A3"
            Cell cell = worksheet.Cells.Find("=A1&A3", null, options);
            Console.WriteLine("Found cell with exact formula match: " + (cell != null ? cell.Name : "null"));

            // Изменить на частичное совпадение
            options.LookAtType = LookAtType.Contains;
            cell = worksheet.Cells.Find("A3", null, options);
            Console.WriteLine("Found cell containing 'A3' in formula: " + (cell != null ? cell.Name : "null"));
        }
    }
}
```

### См. также

* enum [LookAtType](../../lookattype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


