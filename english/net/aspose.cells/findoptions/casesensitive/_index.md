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
            findoptions.LookInType = LookInType.Formulas;
            findoptions.CaseSensitive = true;
            Cell cell = cells.Find("abc", null, findoptions);
            AssertHelper.AreEqual(2, cell.Row, "cell.Row");
            AssertHelper.AreEqual(2, cell.Column, "cell.Column");
        }
```

### See Also

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


