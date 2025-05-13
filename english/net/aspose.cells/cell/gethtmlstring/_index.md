---
title: Cell.GetHtmlString
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the html string which contains data and some formats in this cell
type: docs
url: /net/aspose.cells/cell/gethtmlstring/
---
## Cell.GetHtmlString method

Gets the html string which contains data and some formats in this cell.

```csharp
public string GetHtmlString(bool html5)
```

| Parameter | Type | Description |
| --- | --- | --- |
| html5 | Boolean | Indicates whether the value is compatible for html5 |

### Examples

```csharp
// Called: Assert.AreEqual("<div><span Style=\"FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #000000;VERTICAL-ALIGN: bottom;\">asd</span><span Style=\"FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #ff0000;VERTICAL-ALIGN: bottom;\">fasdf</span><span Style=\"FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #000000;VERTICAL-ALIGN: bottom;\">sdf</span></div>", cell.GetHtmlString(true));
public void Cell_Method_GetHtmlString()
{


    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Cell cell = wb.Worksheets[0].Cells["B2"];
    Assert.AreEqual("<Font Style=\"FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #000000;VERTICAL-ALIGN: bottom;\">asd</Font><Font Style=\"FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #ff0000;VERTICAL-ALIGN: bottom;\">fasdf</Font><Font Style=\"FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #000000;VERTICAL-ALIGN: bottom;\">sdf</Font>", cell.HtmlString);
    Assert.AreEqual("<div><span Style=\"FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #000000;VERTICAL-ALIGN: bottom;\">asd</span><span Style=\"FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #ff0000;VERTICAL-ALIGN: bottom;\">fasdf</span><span Style=\"FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #000000;VERTICAL-ALIGN: bottom;\">sdf</span></div>", cell.GetHtmlString(true));
    Assert.AreEqual("<Font Style=\"FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #000000;VERTICAL-ALIGN: bottom;\"></Font>", wb.Worksheets[0].Cells["A1"].HtmlString);
    wb.Save(Constants.destPath + "example.html");
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


