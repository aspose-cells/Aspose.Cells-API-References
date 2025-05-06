---
title: Workbook.HasRevisions
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets if the workbook has any tracked changes
type: docs
url: /net/aspose.cells/workbook/hasrevisions/
---
## Workbook.HasRevisions property

Gets if the workbook has any tracked changes

```csharp
public bool HasRevisions { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.HasRevisions);
[Test]
        public void Property_HasRevisions()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet41326.xlsx&quot;);
            Assert.IsTrue(workbook.HasRevisions);
            workbook.Save(Constants.destPath + &quot;CELLSNET49983.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET49983.xlsx&quot;);
            Assert.IsTrue(workbook.HasRevisions);
            workbook.Save(Constants.destPath + &quot;CELLSNET49983.xlsb&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET49983.xlsb&quot;);
            Assert.IsTrue(workbook.HasRevisions);
            workbook.Save(Constants.destPath + &quot;CELLSNET49983.xlsx&quot;);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


