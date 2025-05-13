---
title: FindOptions.LookInType
second_title: Aspose.Cells for .NET API Reference
description: FindOptions property. Look in type
type: docs
url: /net/aspose.cells/findoptions/lookintype/
---
## FindOptions.LookInType property

Look in type.

```csharp
public LookInType LookInType { get; set; }
```

### Examples

```csharp
// Called: { LookInType = LookInType.OnlyFormulas, LookAtType = LookAtType.Contains });
private void FindOptions_Property_LookInType(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells.Find("A1", null, new FindOptions()
            { LookInType = LookInType.OnlyFormulas, LookAtType = LookAtType.Contains });
            testAreEqual(1, cell.Row, caseName);
            testAreEqual(1, cell.Column, caseName);
        }
```

### See Also

* enum [LookInType](../../lookintype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


