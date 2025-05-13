---
title: ThreadedCommentAuthorCollection.CurrentPerson
second_title: Aspose.Cells for .NET API Reference
description: ThreadedCommentAuthorCollection property. Gets and sets the current user
type: docs
url: /net/aspose.cells/threadedcommentauthorcollection/currentperson/
---
## ThreadedCommentAuthorCollection.CurrentPerson property

Gets and sets the current user.

```csharp
public ThreadedCommentAuthor CurrentPerson { get; set; }
```

### Examples

```csharp
// Called: authors.CurrentPerson = author;
public static void ThreadedCommentAuthorCollection_Property_CurrentPerson()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the ThreadedCommentAuthorCollection
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

            // Add a new threaded comment author
            int authorIndex = authors.Add("John Doe", "john.doe@example.com", "providerId123");

            // Retrieve the added author
            ThreadedCommentAuthor author = authors[authorIndex];

            // Set the current person
            authors.CurrentPerson = author;

            // Display the current person details
            Console.WriteLine("Current Person: " + authors.CurrentPerson.Name);

            // Save the workbook
            workbook.Save("ThreadedCommentAuthorCollectionExample.xlsx");

            return;
        }
```

### See Also

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


