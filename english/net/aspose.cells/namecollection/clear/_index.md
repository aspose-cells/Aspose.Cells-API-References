---
title: NameCollection.Clear
second_title: Aspose.Cells for .NET API Reference
description: NameCollection method. Remove all defined names which are not referenced by the formulas and data source. If the defined name is referred we only set Name.ReferTo as null and hide them
type: docs
url: /net/aspose.cells/namecollection/clear/
---
## NameCollection.Clear method

Remove all defined names which are not referenced by the formulas and data source. If the defined name is referred, we only set Name.ReferTo as null and hide them.

```csharp
public void Clear()
```

### Examples

```csharp
// Called: workbook.Worksheets.Names.Clear();
[Test]
        public void Method_Clear()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Test_192442.xls&quot;);
            workbook.Worksheets.Names.Clear();
            workbook.Save(Constants.destPath + &quot;Test_192442.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;Test_192442.xls&quot;);
        }
```

### See Also

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


