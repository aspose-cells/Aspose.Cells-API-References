---
title: BorderCollection.SetColor
second_title: Aspose.Cells for .NET API Reference
description: BorderCollection method. Sets the Color of all borders in the collection
type: docs
url: /net/aspose.cells/bordercollection/setcolor/
---
## BorderCollection.SetColor method

Sets the Color of all borders in the collection.

```csharp
public void SetColor(Color color)
```

| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | Borders' Color. |

### Examples

```csharp
// Called: style.Borders.SetColor(Color.Black);
[Test]
		public void Method_Color_()
		{
			
			Workbook excel = new Workbook();
			string designerFile = sourcePath + "Northwind.xls";	
            excel = new Workbook(designerFile);

			Worksheet sheet = excel.Worksheets["Sheet5"];
			sheet.Name = "Employee Sales UK";
			Cells cells = sheet.Cells;
			
			sheet = excel.Worksheets["Sheet6"];
			cells = sheet.Cells;
			sheet.Name = "Employee Sales USA";
			
			ReadEmployees();
			DataTable[] dtSales = this.CreateDataResult();

			int currentUKRow = 6;
			int currentUSARow = 6;

			int styleIndex;
			Style style;

			
            style = excel.CreateStyle();
			style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Double;
			style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Double;
			style.Borders.SetColor(Color.Black);
			style.Font.Size = 12;
			style.Font.IsBold = true;
			style.IsTextWrapped = true;
			style.HorizontalAlignment = TextAlignmentType.Center;
			style.Name = "HeaderStyle";

			for(int i = 0; i < this.dataTable1.Rows.Count; i ++)
			{
				string employeeName = (string)this.dataTable1.Rows[i]["LastName"] + ","
					+ (string)this.dataTable1.Rows[i]["FirstName"];
				if(this.dataTable1.Rows[i]["Country"].ToString() == "UK")
				{
					sheet = excel.Worksheets["Employee Sales UK"];
					cells = sheet.Cells;

					cells[currentUKRow - 2, 0].PutValue("Salesperson:" + employeeName);
					style = excel.CreateStyle();
                    style.Font.IsBold = true;
					style.Font.Size = 12;

					cells[currentUKRow - 2, 0].SetStyle(style);
					
					if((decimal)this.dataTable1.Rows[i]["TotalSales"] > 5000)
					{
						cells[currentUKRow - 2, 3].PutValue("Exceeded Goal!");
						style = excel.CreateStyle();

                        Aspose.Cells.Font font = style.Font;
						font.Color = Color.Red;
						font.IsItalic = true;
						font.Size = 12;
						font.IsBold = true;

						cells[currentUKRow - 2, 3].SetStyle(style);
					}
					cells.SetRowHeight(currentUKRow - 2, 19);
					cells.SetRowHeight(currentUKRow - 1, 4);
					cells.SetRowHeight(currentUKRow, 48);

					style = excel.GetNamedStyle("HeaderStyle");
					for(int j = 1; j < 5; j++)
						cells[currentUKRow, (byte)j].SetStyle(style);
					cells[currentUKRow, 1].PutValue("Order ID:");
					cells[currentUKRow, 2].PutValue("Sales Amount:");
					cells[currentUKRow, 3].PutValue("Percent of Salesperson's Total:");
					cells[currentUKRow, 4].PutValue("Percent of Country Total:");
					currentUKRow ++;

					cells.ImportDataTable(dtSales[i], false, currentUKRow, 1);
					string startCellName1 = CellsHelper.CellIndexToName(currentUKRow, 2);
					string startCellName2 = CellsHelper.CellIndexToName(currentUKRow, 4);
					
					currentUKRow += dtSales[i].Rows.Count - 1;
					string endCellName1 = CellsHelper.CellIndexToName(currentUKRow, 2);
					string endCellName2 = CellsHelper.CellIndexToName(currentUKRow, 4);
					
					cells[currentUKRow + 1, 2].Formula = "=sum(" + startCellName1 + ":" 
						+ endCellName1 +")";

					cells[currentUKRow + 1, 4].Formula = "=sum(" + startCellName2 + ":" 
						+ endCellName2 +")";

					currentUKRow += 4;

				}
				else
				{
					sheet = excel.Worksheets["Employee Sales USA"];
					cells = sheet.Cells;

					cells[currentUSARow - 2, 0].PutValue("Salesperson:" + employeeName);

					style = excel.CreateStyle();
                    style.Font.IsBold = true;
					style.Font.Size = 12;
					cells[currentUSARow - 2, 0].SetStyle(style);
					
					if((decimal)this.dataTable1.Rows[i]["TotalSales"] > 5000)
					{
						style = excel.CreateStyle();

                        cells[currentUSARow - 2, 3].PutValue("Exceeded Goal!");
						Aspose.Cells.Font font = style.Font;
						font.Color = Color.Red;
						font.IsItalic = true;
						font.Size = 12;
						font.IsBold = true;
						
						cells[currentUSARow - 2, 3].SetStyle(style);
					}
					cells.SetRowHeight(currentUSARow - 2, 19);
					cells.SetRowHeight(currentUSARow - 1, 4);
					cells.SetRowHeight(currentUSARow, 48);

					style = excel.GetNamedStyle("HeaderStyle");
					for(int j = 1; j < 5; j++)
						cells[currentUSARow, (byte)j].SetStyle(style);
					cells[currentUSARow, 1].PutValue("Order ID:");
					cells[currentUSARow, 2].PutValue("Sales Amount:");
					cells[currentUSARow, 3].PutValue("Percent of Salesperson's Total:");
					cells[currentUSARow, 4].PutValue("Percent of Country Total:");
					currentUSARow ++;

					cells.ImportDataTable(dtSales[i], false, currentUSARow, 1);

					string startCellName1 = CellsHelper.CellIndexToName(currentUSARow, 2);
					string startCellName2 = CellsHelper.CellIndexToName(currentUSARow, 4);
					
					currentUSARow += dtSales[i].Rows.Count - 1;
					string endCellName1 = CellsHelper.CellIndexToName(currentUSARow, 2);
					string endCellName2 = CellsHelper.CellIndexToName(currentUSARow, 4);
					
					cells[currentUSARow + 1, 2].Formula = "=sum(" + startCellName1 + ":" 
						+ endCellName1 +")";

					cells[currentUSARow + 1, 4].Formula = "=sum(" + startCellName2 + ":" 
						+ endCellName2 +")";

					currentUSARow += 4;
				}
			}
			for(int i = 0; i < excel.Worksheets.Count ; i ++)
			{
				sheet = excel.Worksheets[i];
				if(sheet.Name != "Employee Sales UK" && sheet.Name != "Employee Sales USA")
				{
					excel.Worksheets.RemoveAt(i);
					i --;
				}

			}
			excel.Save(destPath + "EmployeeSales.xls");		
		}
```

### See Also

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


