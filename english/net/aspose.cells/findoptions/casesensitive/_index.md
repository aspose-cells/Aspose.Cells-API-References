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
// Called: ContainsFindOptions.CaseSensitive = true;
private void FindOptions_Property_CaseSensitive(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            ContainsFindOptions.CaseSensitive = true;
            Cell cell = cells.Find("bc", null, ContainsFindOptions);
            testAreEqual(null, cell, caseName);
        }
```

### See Also

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


