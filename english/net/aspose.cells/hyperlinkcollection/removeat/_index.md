---
title: HyperlinkCollection.RemoveAt
second_title: Aspose.Cells for .NET API Reference
description: HyperlinkCollection method. Remove the hyperlink at the specified index in this collection
type: docs
url: /net/aspose.cells/hyperlinkcollection/removeat/
---
## HyperlinkCollection.RemoveAt method

Remove the hyperlink at the specified index in this collection.

```csharp
public void RemoveAt(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The zero based index of the element. |

### Examples

```csharp
// Called: hyperlinks.RemoveAt(0);
public static void Method_Int32_()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[0];

            // Get Hyperlinks Collection
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Adding a hyperlink to a URL at "A1" cell
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Adding another hyperlink to a URL at "B1" cell
            hyperlinks.Add("B1", 1, 1, "http://www.example.com");

            // Adding a hyperlink with a range of cells
            hyperlinks.Add("C1", 1, 2, "http://www.test.com");

            // Adding a hyperlink with a specific text to display and screen tip
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            // Removing the first hyperlink
            hyperlinks.RemoveAt(0);

            // Clearing all hyperlinks
            hyperlinks.Clear();

            // Adding a hyperlink again to demonstrate saving
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Saving the Excel file
            workbook.Save("HyperlinkCollectionExample.xlsx");
            workbook.Save("HyperlinkCollectionExample.pdf");
            return;
        }
```

### See Also

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


