---
title: TableStyleElement.GetElementStyle
second_title: Aspose.Cells for .NET API Reference
description: TableStyleElement method. Gets the element style
type: docs
url: /net/aspose.cells.tables/tablestyleelement/getelementstyle/
---
## TableStyleElement.GetElementStyle method

Gets the element style.

```csharp
public Style GetElementStyle()
```

### Return Value

Returns the [`Style`](../../../aspose.cells/style/) object.

### Examples

```csharp
// Called: Style eStyle = style.TableStyleElements[TableStyleElementType.WholeTable].GetElementStyle();
[Test]
        public void Method_GetElementStyle()
        {
            //-2171174
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet45252.xls&quot;);
            TableStyle style = workbook.Worksheets.TableStyles[0];
            Style eStyle = style.TableStyleElements[TableStyleElementType.WholeTable].GetElementStyle();
            Assert.AreEqual(eStyle.Borders[BorderType.Horizontal].Color.ToArgb(), -2171174);
            Assert.AreEqual(eStyle.Borders[BorderType.Horizontal].LineStyle, CellBorderType.Medium);
            workbook.Save(Constants.destPath + &quot;CellsNet45252.xlsx&quot;);
        }
```

### See Also

* class [Style](../../../aspose.cells/style/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


