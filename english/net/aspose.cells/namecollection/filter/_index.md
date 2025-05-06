---
title: NameCollection.Filter
second_title: Aspose.Cells for .NET API Reference
description: NameCollection method. Gets all defined name by scope
type: docs
url: /net/aspose.cells/namecollection/filter/
---
## NameCollection.Filter method

Gets all defined name by scope.

```csharp
public Name[] Filter(NameScopeType type, int sheetIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | NameScopeType | The scope type. |
| sheetIndex | Int32 | The sheet index. Only effects when scope type is Worksheet |

### Examples

```csharp
// Called: Assert.AreEqual(2, workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, -1).Length);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET50332.xlsx&quot;);

            Assert.AreEqual(1,workbook.Worksheets.Names.Filter(NameScopeType.Workbook, -1).Length);
            Assert.AreEqual(2, workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, -1).Length);
            Assert.AreEqual(1, workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, 1).Length);
            // Save the workbook
            workbook.Save(Constants.destPath + &quot;dest.xlsx&quot;);
        }
```

### See Also

* class [Name](../../name/)
* enum [NameScopeType](../../namescopetype/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


