---
title: FindOptions.CaseSensitive
second_title: Aspose.Cells for .NET API Reference
description: FindOptions property. Indicates if the searched string is case sensitive
type: docs
url: /net/aspose.cells/findoptions/casesensitive/
---
## FindOptions.CaseSensitive property

Indicates if the searched string is case sensitive.

```csharp
public bool CaseSensitive { get; set; }
```

### Examples

```csharp
// Called: findoptions.CaseSensitive = true;
private void Property_CaseSensitive(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            FindOptions findoptions = new FindOptions();
            findoptions.LookAtType = LookAtType.StartWith;
            findoptions.CaseSensitive = true;
            Cell cell = cells.Find(&quot;abc&quot;, null, findoptions);
            AssertHelper.AreEqual(2, cell.Row, &quot;cell.Row&quot;);
            AssertHelper.AreEqual(2, cell.Column, &quot;cell.Column&quot;);
        }
```

### See Also

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


