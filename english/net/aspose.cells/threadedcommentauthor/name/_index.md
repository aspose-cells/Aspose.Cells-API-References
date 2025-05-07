---
title: ThreadedCommentAuthor.Name
second_title: Aspose.Cells for .NET API Reference
description: ThreadedCommentAuthor property. Gets and sets the name
type: docs
url: /net/aspose.cells/threadedcommentauthor/name/
---
## ThreadedCommentAuthor.Name property

Gets and sets the name.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine("Current Person: " + authors.CurrentPerson.Name);
public static void Property_Name()
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

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


