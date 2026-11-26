---
title: "Comment.HeightInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Представляет высоту комментария в дюймах"
type: docs
url: /ru/net/aspose.cells/comment/heightinch/
---
## Comment.HeightInch property

Представляет высоту комментария в дюймах.

```csharp
public double HeightInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            comment.HeightInch = 1.5;
            Console.WriteLine("Comment height set to: " + comment.HeightInch + " inches");
        }
    }
}
```

### См. также

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


