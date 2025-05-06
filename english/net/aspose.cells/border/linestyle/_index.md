---
title: Border.LineStyle
second_title: Aspose.Cells for .NET API Reference
description: Border property. Gets or sets the cell border type
type: docs
url: /net/aspose.cells/border/linestyle/
---
## Border.LineStyle property

Gets or sets the cell border type.

```csharp
public CellBorderType LineStyle { get; set; }
```

### Examples

```csharp
// Called: style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
private void Property_LineStyle(Workbook excel)
		{



            Aspose.Cells.Style style = excel.Property_LineStyle();


            style.Name = &quot;Box&quot;;

			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.None;

			style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.None;


			style = excel.Property_LineStyle();

            style.Font.Size = 20;

			style.Font.IsBold = true;

			style.Name = &quot;H1&quot;;



			style = excel.Property_LineStyle();

            style.Font.Size = 16;

			style.Font.IsBold = true;

			style.Name = &quot;H2&quot;;



			style = excel.Property_LineStyle();

            style.Font.Size = 12;

			style.Font.IsBold = true;

			style.Name = &quot;H3&quot;;



			style = excel.Property_LineStyle();

            style.Font.Size = 7;

			style.Font.IsBold = false;

			style.Name = &quot;SmallTable&quot;;

			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.None;

			style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.None;



			style = excel.Property_LineStyle();

            style.Font.Size = 7;

			style.Font.IsBold = false;

			style.ForegroundColor = Color.Blue;

			style.Font.Color = Color.White;

			style.Pattern = BackgroundType.Solid;

			style.Name = &quot;SmallTableBlue&quot;;

			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.None;

			style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.None;



			style = excel.Property_LineStyle();

            style.Font.Size = 7;

			style.Font.IsBold = false;

			style.ForegroundColor = Color.Red;

			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.None;

			style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.None;

			style.Font.Color = Color.White;

			style.Pattern = BackgroundType.Solid;

			style.Name = &quot;SmallTableRed&quot;;



			style = excel.Property_LineStyle();

            style.Font.Size = 7;

			style.Font.IsBold = false;

			excel.ChangePalette(Color.LightBlue, 55);

			style.ForegroundColor = Color.LightBlue;

			style.Font.Color = Color.Black;

			style.Pattern = BackgroundType.Solid;

			style.Name = &quot;SmallTableLightBlue&quot;;

			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.None;

			style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.None;



			style = excel.Property_LineStyle();

            style.Font.Size = 7;

			style.Font.IsBold = false;

			excel.ChangePalette(Color.Pink, 54);

			style.ForegroundColor = Color.Pink;

			style.Font.Color = Color.Black;

			style.Pattern = BackgroundType.Solid;

			style.Name = &quot;SmallTablePink&quot;;

			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.None;

			style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.None;



			style = excel.Property_LineStyle();

            style.Font.Size = 7;

			style.Font.IsBold = false;

			style.ForegroundColor = Color.Yellow;

			style.Font.Color = Color.Black;

			style.Pattern = BackgroundType.Solid;

			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.None;

			style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.None;



			style.Name = &quot;SmallTableYellow&quot;;



			style = excel.Property_LineStyle();

            style.Font.Size = 7;

			style.Font.IsBold = true;

			style.Name = &quot;SmallTableTitle&quot;;

			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.None;

			style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.None;



			style = excel.Property_LineStyle();

            style.Font.Size = 9;

			style.Font.IsBold = false;

			style.Name = &quot;H4&quot;;



			style = excel.Property_LineStyle();

            style.Font.Size = 9;

			style.Font.IsBold = true;

			style.Name = &quot;H4Bold&quot;;







			style = excel.Property_LineStyle();

            style.Font.Size = 6;

			style.Font.IsBold = false;

			style.Name = &quot;Table&quot;;

			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.None;

			style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.None;



			style = excel.Property_LineStyle();

            style.Font.Size = 6;

			style.Font.IsBold = false;

			style.ForegroundColor = Color.Blue;

			style.Font.Color = Color.White;

			style.Pattern = BackgroundType.Solid;

			style.Name = &quot;TableBlue&quot;;

			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.None;

			style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.None;




			style = excel.Property_LineStyle();

            style.Font.Size = 6;

			style.Font.IsBold = false;

			style.ForegroundColor = Color.Red;

			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.None;

			style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.None;

			style.Font.Color = Color.White;

			style.Pattern = BackgroundType.Solid;

			style.Name = &quot;TableRed&quot;;



			style = excel.Property_LineStyle();

            style.Font.Size = 6;

			style.Font.IsBold = false;

			style.ForegroundColor = Color.LightBlue;

			style.Font.Color = Color.Black;

			style.Pattern = BackgroundType.Solid;

			style.Name = &quot;TableLightBlue&quot;;

			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.None;

			style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.None;




			style = excel.Property_LineStyle();

            style.Font.Size = 6;

			style.Font.IsBold = false;

			style.ForegroundColor = Color.Pink;

			style.Font.Color = Color.Black;

			style.Pattern = BackgroundType.Solid;

			style.Name = &quot;TablePink&quot;;

			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.None;

			style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.None;



			style = excel.Property_LineStyle();

            style.Font.Size = 6;

			style.Font.IsBold = false;

			style.ForegroundColor = Color.Yellow;

			style.Font.Color = Color.Black;

			style.Pattern = BackgroundType.Solid;

			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.None;

			style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.None;

			style.Name = &quot;TableYellow&quot;;



			style = excel.Property_LineStyle();

            style.Font.Size = 6;

			style.Font.IsBold = false;

			excel.ChangePalette(Color.LightGray, 54);

			style.ForegroundColor = Color.LightGray;

			style.Font.Color = Color.Black;

			style.Pattern = BackgroundType.Solid;

			style.Name = &quot;TableTenor&quot;;

			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

			style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.None;

			style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.None;

		}
```

### See Also

* enum [CellBorderType](../../cellbordertype/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


