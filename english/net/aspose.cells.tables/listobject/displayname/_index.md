---
title: ListObject.DisplayName
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets the display name
type: docs
url: /net/aspose.cells.tables/listobject/displayname/
---
## ListObject.DisplayName property

Gets and sets the display name.

```csharp
public string DisplayName { get; set; }
```

### Examples

```csharp
// Called: listObjects[0].DisplayName = &amp;quot;TestTable&amp;quot;;
[Test]
        public void Property_DisplayName()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue(&quot;a&quot;);
            cells[1, 0].PutValue(1);
            cells[2, 0].PutValue(2);
            cells[3, 0].PutValue(3);
            cells[0, 1].PutValue(&quot;b&quot;);
            cells[1, 1].PutValue(4);
            cells[2, 1].PutValue(5);
            cells[3, 1].PutValue(6);

            ListObjectCollection listObjects = workbook.Worksheets[0].ListObjects;
            listObjects.Add(&quot;A1&quot;, &quot;B4&quot;, true);
            listObjects[0].DisplayName = &quot;TestTable&quot;;
            workbook.Save(Constants.destPath + &quot;ListObject_DisplayName_001.xls&quot;);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


