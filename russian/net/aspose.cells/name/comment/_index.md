---
title: "Name.Comment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Name property. Получает и задает комментарий имени. Применяется только к Excel 2007 и более новым версиям"
type: docs
url: /ru/net/aspose.cells/name/comment/
---
## Name.Comment property

Получает и задаёт комментарий к имени. Применяется только для Excel 2007 и более новых версий.

```csharp
public string Comment { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyCommentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте именованный диапазон с комментарием
            int index = workbook.Worksheets.Names.Add("TestRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
            namedRange.Comment = "This is a test named range";
            
            // Сохраните книгу
            workbook.Save("NamedRangeWithComment.xlsx");
            
            // Загрузите сохранённую книгу, чтобы проверить комментарий
            Workbook loadedWorkbook = new Workbook("NamedRangeWithComment.xlsx");
            Name loadedNamedRange = loadedWorkbook.Worksheets.Names[0];
            
            // Выведите комментарий, чтобы продемонстрировать функциональность
            Console.WriteLine("Named Range Comment: " + loadedNamedRange.Comment);
        }
    }
}
```

### См. также

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


