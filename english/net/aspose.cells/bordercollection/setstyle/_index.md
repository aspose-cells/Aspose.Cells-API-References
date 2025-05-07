---
title: BorderCollection.SetStyle
second_title: Aspose.Cells for .NET API Reference
description: BorderCollection method. Sets the style of all borders of the collection
type: docs
url: /net/aspose.cells/bordercollection/setstyle/
---
## BorderCollection.SetStyle method

Sets the style of all borders of the collection.

```csharp
public void SetStyle(CellBorderType style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | CellBorderType | Borders' style |

### Examples

```csharp
// Called: style.Borders.SetStyle(CellBorderType.None);
[Test]
		public void Method_CellBorderType_()
		{
            Workbook excel = new Workbook(Constants.sourcePath + "mergecellborder.xls");
			Style style = excel.Worksheets[0].Cells[1,1].GetStyle();

			style.Borders.SetStyle(CellBorderType.None);
			

			excel.Worksheets[0].Cells[1,1].SetStyle(style);

			style = excel.Worksheets[0].Cells[1,2].GetStyle();

			style.Borders.SetStyle(CellBorderType.None);
			
			excel.Worksheets[0].Cells[1,2].SetStyle(style);

            excel.Save(Constants.destPath + "removedborder.xls");

		}
```

### See Also

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


