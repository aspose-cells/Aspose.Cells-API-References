---
title: "ThreadedCommentAuthorCollection.CurrentPerson"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreadedCommentAuthorCollection. Obtiene y establece el usuario actual"
type: docs
url: /es/net/aspose.cells/threadedcommentauthorcollection/currentperson/
---
## ThreadedCommentAuthorCollection.CurrentPerson property

Obtiene y establece el usuario actual.

```csharp
public ThreadedCommentAuthor CurrentPerson { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorCollectionPropertyCurrentPersonDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            int authorIndex = authors.Add("Jane Smith", "jane.smith@example.com", "provider456");
            ThreadedCommentAuthor author = authors[authorIndex];

            authors.CurrentPerson = author;
            Console.WriteLine("Current Person: " + authors.CurrentPerson.Name);

            workbook.Save("ThreadedCommentAuthorsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


