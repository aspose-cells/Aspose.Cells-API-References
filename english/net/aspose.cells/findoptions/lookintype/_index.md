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
private void Property_LookInType(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            string formula = "=SUM(A1,B1)";
            cells[1, 1].Formula = formula;
            Cell cell = cells.Find("=SUM(A1,B2)", null, new FindOptions()
            { LookInType = LookInType.OnlyFormulas, LookAtType = LookAtType.Contains });
            testAreEqual(null, cell, caseName);
        }
```

### See Also

* enum [LookInType](../../lookintype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


