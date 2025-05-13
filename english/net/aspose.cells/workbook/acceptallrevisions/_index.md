---
title: Workbook.AcceptAllRevisions
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Accepts all tracked changes in the workbook
type: docs
url: /net/aspose.cells/workbook/acceptallrevisions/
---
## Workbook.AcceptAllRevisions method

Accepts all tracked changes in the workbook.

```csharp
public void AcceptAllRevisions()
```

### Examples

```csharp
// Called: workbook.AcceptAllRevisions();
public void Workbook_Method_AcceptAllRevisions()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual(workbook.HasRevisions, true);
    workbook.AcceptAllRevisions();
    using(FileStream fs = File.Create(Constants.destPath +"CellsNet41326"))
    {
                
        workbook.Save(fs,SaveFormat.Xlsx);
    }
    workbook = new Workbook(Constants.destPath + "CellsNet41326");
    Assert.AreEqual(workbook.HasRevisions, false);
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


