---
title: "ThreadedCommentAuthorCollection.CurrentPerson"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreadedCommentAuthorCollection. Obtient et définit l'utilisateur actuel"
type: docs
url: /fr/net/aspose.cells/threadedcommentauthorcollection/currentperson/
---
## ThreadedCommentAuthorCollection.CurrentPerson property

Obtient et définit l'utilisateur actuel.

```csharp
public ThreadedCommentAuthor CurrentPerson { get; set; }
```

### Exemples

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

### Voir aussi

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


