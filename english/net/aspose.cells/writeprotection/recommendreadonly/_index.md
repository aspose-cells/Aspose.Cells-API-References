---
title: WriteProtection.RecommendReadOnly
second_title: Aspose.Cells for .NET API Reference
description: WriteProtection property. Indicates if the Read Only Recommended option is selected
type: docs
url: /net/aspose.cells/writeprotection/recommendreadonly/
---
## WriteProtection.RecommendReadOnly property

Indicates if the Read Only Recommended option is selected.

```csharp
public bool RecommendReadOnly { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Settings.WriteProtection.RecommendReadOnly);
[Test]
        public void Property_RecommendReadOnly()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet45576.xlsx&quot;);
           Assert.IsTrue(workbook.Settings.WriteProtection.RecommendReadOnly);
           Assert.IsFalse(workbook.Settings.WriteProtection.IsWriteProtected);
           workbook.Save(Constants.destPath + &quot;CellsNet45576.xls&quot;);
           workbook = new Workbook(Constants.destPath + &quot;CellsNet45576.xls&quot;);
           Assert.IsTrue(workbook.Settings.WriteProtection.RecommendReadOnly);
           Assert.IsFalse(workbook.Settings.WriteProtection.IsWriteProtected);
        }
```

### See Also

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


