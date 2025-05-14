---
title: PageSetup.FitToPagesWide
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the number of pages wide the worksheet will be scaled to when its printed. The default value is 1
type: docs
url: /net/aspose.cells/pagesetup/fittopageswide/
---
## PageSetup.FitToPagesWide property

Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1.

```csharp
public int FitToPagesWide { get; set; }
```

### Remarks

You have to set FitToPagesTall as zero if you want to fit all columns on one page.

### Examples

```csharp
// Called: excel.Worksheets[0].PageSetup.FitToPagesWide = 0;
		public void PageSetup_Property_FitToPagesWide()
		{
			Workbook excel = new Workbook();
			this.CreateStyle(excel);
            Aspose.Cells.Style style = excel.CreateStyle();
			//excel.ChangePalette(Color.Blue, 55); 
			style.ForegroundColor = Color.Blue;
			style.BackgroundColor = Color.Red;
			style.Pattern = BackgroundType.DiagonalStripe; 
			
			style.Name = "Header5"; 

			style = excel.GetNamedStyle("Table");
			excel.Worksheets[0].Cells["A1"].PutValue(12.3456);
			excel.Worksheets[0].Cells["A1"].SetStyle(style);

			//excel.Worksheets[0].Cells["A1"].Style.Number = 2;

			excel.Worksheets[0].Cells["B1"].SetStyle(excel.GetNamedStyle("Header5"));


			excel.Worksheets[0].Cells["c1"].SetStyle(excel.GetNamedStyle("Box"));

			excel.Worksheets[0].Cells["d1"].SetStyle(excel.GetNamedStyle("H1"));
			excel.Worksheets[0].Cells["d1"].PutValue("hello");

			excel.Worksheets[0].Cells["e1"].SetStyle(excel.GetNamedStyle("H3"));
			excel.Worksheets[0].Cells["e1"].PutValue("world");


			excel.Worksheets[0].PageSetup.FitToPagesTall = 1;
			excel.Worksheets[0].PageSetup.FitToPagesWide = 0;

			excel.Save(Constants.destPath + "\\styles.xls");
		}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


