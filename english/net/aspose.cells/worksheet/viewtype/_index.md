---
title: Worksheet.ViewType
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets and sets the view type
type: docs
url: /net/aspose.cells/worksheet/viewtype/
---
## Worksheet.ViewType property

Gets and sets the view type.

```csharp
public ViewType ViewType { get; set; }
```

### Examples

```csharp
// Called: workbook.Worksheets[0].ViewType = ViewType.PageLayoutView;
public void Worksheet_Property_ViewType()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets[0].ViewType = ViewType.PageLayoutView;
    workbook.Worksheets[0].IsRulerVisible = true;
    workbook.Save(Constants.destPath + "example.xlsb");
    workbook = new Workbook(Constants.destPath + "example.xlsb");
    Assert.IsTrue(workbook.Worksheets[0].IsRulerVisible);
}
```

### See Also

* enum [ViewType](../../viewtype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


