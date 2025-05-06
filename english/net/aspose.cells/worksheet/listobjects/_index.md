---
title: Worksheet.ListObjects
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets all ListObjects in this worksheet
type: docs
url: /net/aspose.cells/worksheet/listobjects/
---
## Worksheet.ListObjects property

Gets all ListObjects in this worksheet.

```csharp
public ListObjectCollection ListObjects { get; }
```

### Examples

```csharp
// Called: ListObject list = sheet.ListObjects[0];
[Test]
        public void Property_ListObjects()
        {
            Workbook book = new Workbook(Constants.sourcePath + &quot;CellsJava41389.xlsx&quot;);
            Worksheet sheet = book.Worksheets[0];
            int index = sheet.ListObjects.Add(&quot;A1&quot;, &quot;B9&quot;, true);
            ListObject list = sheet.ListObjects[0];
            Assert.AreEqual(8, list.EndRow);
            list.ShowTotals = (true);
            Assert.AreEqual(9, list.EndRow);
            book.Save(Constants.destPath + &quot;CellsJava41389.xlsx&quot;);
        }
```

### See Also

* class [ListObjectCollection](../../../aspose.cells.tables/listobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


