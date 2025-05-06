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
// Called: Cell cell = cells.Find(formula, null, new FindOptions() { LookInType = LookInType.OnlyFormulas, LookAtType = LookAtType.EntireContent });
private void Property_LookInType(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            string formula = &quot;=SUM(A1,B1)&quot;;
            Cell cell = cells.Find(formula, null, new FindOptions() { LookInType = LookInType.OnlyFormulas, LookAtType = LookAtType.EntireContent });
            testAreEqual(1, cell.Row, caseName);
            testAreEqual(1, cell.Column, caseName);
        }
```

### See Also

* enum [LookInType](../../lookintype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


