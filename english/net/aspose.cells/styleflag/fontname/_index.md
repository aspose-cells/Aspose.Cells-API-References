---
title: StyleFlag.FontName
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Font name setting will be applied
type: docs
url: /net/aspose.cells/styleflag/fontname/
---
## StyleFlag.FontName property

Font name setting will be applied.

```csharp
public bool FontName { get; set; }
```

### Examples

```csharp
// Called: flag.FontName = true;
		public void StyleFlag_Property_FontName()
		{
			Workbook excel = new Workbook();
			string designerFile = sourcePath + "Northwind.xls";
			
            excel = new Workbook(designerFile);
			
			ReadCategory();
			DataTable dataTable2 = new DataTable();
			
			Worksheet sheet = excel.Worksheets["Sheet2"];
			sheet.Name = "Catalog";
			Cells cells = sheet.Cells;

			int currentRow = 55;

			//Add LightGray color to color palette
			excel.ChangePalette(Color.LightGray, 55);


            //Set CategoryName style

            Style styleCategoryName = excel.CreateStyle();

            styleCategoryName.Font.Size = 14;
			styleCategoryName.Font.Color = Color.Blue;
			styleCategoryName.Font.IsBold = true;
			styleCategoryName.Font.Name = "Times New Roman";

	
			Style styleDescription = excel.CreateStyle();
            styleDescription.Font.Name = "Times New Roman";
			styleDescription.Font.Color = Color.Blue;
			styleDescription.Font.IsItalic = true;


			Style styleProductName = excel.CreateStyle();
            styleProductName.Font.IsBold = true;


			Style styleTitle = excel.CreateStyle();
            styleTitle.Font.IsBold = true;
			styleTitle.Font.IsItalic = true;
			styleTitle.ForegroundColor = Color.LightGray;
			styleTitle.Pattern = BackgroundType.Solid;


			Style styleNumber = excel.CreateStyle();
            styleNumber.Font.Name = "Times New Roman";
			styleNumber.Number = 8;


            HorizontalPageBreakCollection hPageBreaks = sheet.HorizontalPageBreaks;
			
			string cmdText = "SELECT ProductName, ProductID, QuantityPerUnit, " +
				"UnitPrice FROM Products";
			for(int i = 0; i < this.dataTable1.Rows.Count; i ++)
			{
				currentRow += 2;
				cells.SetRowHeight(currentRow, 20);
				cells[currentRow, 1].SetStyle(styleCategoryName);
				DataRow categoriesRow = this.dataTable1.Rows[i];
				
				//Write CategoryName
				cells[currentRow, 1].PutValue((string)categoriesRow["CategoryName"]);

				//Write Description
				currentRow ++;
				cells[currentRow, 1].PutValue((string)categoriesRow["Description"]);
				cells[currentRow, 1].SetStyle(styleDescription);

				dataTable2.Clear();
				oleDbDataAdapter2.SelectCommand.CommandText = cmdText +" where categoryid = " 
					+ categoriesRow["CategoryID"].ToString();
				oleDbDataAdapter2.Fill(dataTable2);

				currentRow += 2;
				cells.ImportDataTable(dataTable2, true, currentRow, 1);
				
				Aspose.Cells.Range range = cells.CreateRange(currentRow, 1, 1, 4);

				StyleFlag flag = new StyleFlag();
				flag.CellShading = true;
				flag.FontBold = true;
				flag.FontItalic = true;
				range.ApplyStyle(styleTitle, flag);
				
				range = cells.CreateRange(currentRow + 1, 1, dataTable2.Rows.Count, 1);
				flag = new StyleFlag();
				flag.FontBold = true;
				range.ApplyStyle(styleProductName, flag);
				
				range = cells.CreateRange(currentRow + 1, 4, dataTable2.Rows.Count, 1);
				flag = new StyleFlag();
				flag.FontName = true;
				flag.NumberFormat = true;
				range.ApplyStyle(styleNumber, flag);
			
				currentRow += dataTable2.Rows.Count;
				hPageBreaks.Add(currentRow, 0);
			}

			for(int i = 0; i < excel.Worksheets.Count ; i ++)
			{
				sheet = excel.Worksheets[i];
				if(sheet.Name != "Catalog")
				{
					excel.Worksheets.RemoveAt(i);
					i --;
				}

			}
			excel.Save(destPath + "Catalog.xls");
		}
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


