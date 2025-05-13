---
title: TableStyle.TableStyleElements
second_title: Aspose.Cells for .NET API Reference
description: TableStyle property. Gets all elements of the table style
type: docs
url: /net/aspose.cells.tables/tablestyle/tablestyleelements/
---
## TableStyle.TableStyleElements property

Gets all elements of the table style.

```csharp
public TableStyleElementCollection TableStyleElements { get; }
```

### Examples

```csharp
// Called: Style eStyle = style.TableStyleElements[TableStyleElementType.WholeTable].GetElementStyle();
public void TableStyle_Property_TableStyleElements()
{
    //-2171174
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    TableStyle style = workbook.Worksheets.TableStyles[0];
    Style eStyle = style.TableStyleElements[TableStyleElementType.WholeTable].GetElementStyle();
    Assert.AreEqual(eStyle.Borders[BorderType.Horizontal].Color.ToArgb(), -2171174);
    Assert.AreEqual(eStyle.Borders[BorderType.Horizontal].LineStyle, CellBorderType.Medium);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [TableStyleElementCollection](../../tablestyleelementcollection/)
* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


