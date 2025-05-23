---
title: Style.IsModified
second_title: Aspose.Cells for .NET API Reference
description: Style method. Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell
type: docs
url: /net/aspose.cells/style/ismodified/
---
## Style.IsModified method

Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell.

```csharp
public bool IsModified(StyleModifyFlag modifyFlag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| modifyFlag | StyleModifyFlag | Style modified flags |

### Return Value

true if the specified properties have been modified

### Examples

```csharp
// Called: Assert.IsTrue(style.IsModified(StyleModifyFlag.Pattern));
	    public void Style_Method_IsModified()
	    {

            Workbook wb = new Workbook(Constants.sourcePath + "example.xls");
	        Style style = wb.Worksheets[0].Cells["C4"].GetStyle();
            Assert.IsTrue(style.IsModified(StyleModifyFlag.Pattern));
	    }
```

### See Also

* enum [StyleModifyFlag](../../stylemodifyflag/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


