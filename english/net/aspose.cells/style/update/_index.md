---
title: Style.Update
second_title: Aspose.Cells for .NET API Reference
description: Style method. Apply the named style to the styles of the cells which use this named style. It works like clicking the ok button after you finished modifying the style. Only applies for named style
type: docs
url: /net/aspose.cells/style/update/
---
## Style.Update method

Apply the named style to the styles of the cells which use this named style. It works like clicking the "ok" button after you finished modifying the style. Only applies for named style.

```csharp
public void Update()
```

### Examples

```csharp
// Called: style.Update();
public void Style_Method_Update()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    // workbook.ConvertNumericData = false;
    //

    Style style = workbook.GetNamedStyle("Percent");
    style.Number = 3;
    style.Update();
    Assert.AreEqual(workbook.Worksheets[0].Cells["A1"].GetStyle().Number, 3);
            
}
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


