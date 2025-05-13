---
title: Style.Copy
second_title: Aspose.Cells for .NET API Reference
description: Style method. Copies data from another style object
type: docs
url: /net/aspose.cells/style/copy/
---
## Style.Copy method

Copies data from another style object

```csharp
public void Copy(Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | Source Style object |

### Remarks

This method does not copy the name of the style. If you want to copy the name, please call the following codes after copying style: destStyle.Name = style.Name.

### Examples

```csharp
// Called: newbook.DefaultStyle.Copy(workbook.DefaultStyle);
public void Style_Method_Copy()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Workbook newbook = new Workbook();

    newbook.CopyTheme(workbook);
    newbook.DefaultStyle.Copy(workbook.DefaultStyle);

    Worksheet newsheet = newbook.Worksheets[0];
    newsheet.Copy(workbook.Worksheets[0]);
    // newsheet.Shapes[0].ToImage(dir + "dest.jpg", null);
    newbook.Save(Constants.destPath + "example.pdf");
}
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


