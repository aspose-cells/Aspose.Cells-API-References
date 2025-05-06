---
title: FindOptions.IsCaseSensitive
second_title: Aspose.Cells for .NET API Reference
description: FindOptions property. Indicates if the searched string is case sensitive
type: docs
url: /net/aspose.cells/findoptions/iscasesensitive/
---
## FindOptions.IsCaseSensitive property

Indicates if the searched string is case sensitive.

```csharp
[Obsolete("Use FindOptions.CaseSensitive property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsCaseSensitive { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use FindOptions.CaseSensitive property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: findoptions.IsCaseSensitive = true;
private void Property_IsCaseSensitive(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            FindOptions findoptions = new FindOptions();
            findoptions.IsCaseSensitive = true;
            Cell cell = cells.Find(&quot;abc&quot;, null, findoptions);
            AssertHelper.AreEqual(2, cell.Row, &quot;cell.Row&quot;);
            AssertHelper.AreEqual(3, cell.Column, &quot;cell.Column&quot;);
        }
```

### See Also

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


