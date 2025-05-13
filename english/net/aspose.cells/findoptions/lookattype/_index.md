---
title: FindOptions.LookAtType
second_title: Aspose.Cells for .NET API Reference
description: FindOptions property. Look at type
type: docs
url: /net/aspose.cells/findoptions/lookattype/
---
## FindOptions.LookAtType property

Look at type.

```csharp
public LookAtType LookAtType { get; set; }
```

### Remarks

When [`RegexKey`](../regexkey/) is true and user has specified the exact rule for the regex, for performance consideration this property should be set as EntireContent. Otherwise we will refactor the search key to ensure it can be matched according to the specific type. For example, when the type is Contains(this is the default value for this property), we will add wildcards at the beginning and end of the search key automatically. In this case, the regular expressions will become more complex and the performance will also decrease.

### Examples

```csharp
// Called: { LookInType = LookInType.OnlyFormulas, LookAtType = LookAtType.EntireContent });
private void FindOptions_Property_LookAtType(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            Cell previousCell = cells[3, 0];
            Cell cell = cells.Find("", previousCell, new FindOptions()
            { LookInType = LookInType.OnlyFormulas, LookAtType = LookAtType.EntireContent });
            testAreEqual(null, cell, caseName);   
        }
```

### See Also

* enum [LookAtType](../../lookattype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


