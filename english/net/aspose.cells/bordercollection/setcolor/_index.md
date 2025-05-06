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
			string designerFile = sourcePath + &quot;Northwind.xls&quot;;	
            excel = new Workbook(designerFile);

			Worksheet sheet = excel.Worksheets[&quot;Sheet5&quot;];
			sheet.Name = &quot;Employee Sales UK&quot;;
			Cells cells = sheet.Cells;
			
			sheet = excel.Worksheets[&quot;Sheet6&quot;];
			cells = sheet.Cells;
			sheet.Name = &quot;Employee Sales USA&quot;;
			
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
			style.Name = &quot;HeaderStyle&quot;;

			for(int i = 0; i &lt; this.dataTable1.Rows.Count; i ++)
			{
				string employeeName = (string)this.dataTable1.Rows[i][&quot;LastName&quot;] + &quot;,&quot;
					+ (string)this.dataTable1.Rows[i][&quot;FirstName&quot;];
				if(this.dataTable1.Rows[i][&quot;Country&quot;].ToString() == &quot;UK&quot;)
				{
					sheet = excel.Worksheets[&quot;Employee Sales UK&quot;];
					cells = sheet.Cells;

					cells[currentUKRow - 2, 0].PutValue(&quot;Salesperson:&quot; + employeeName);
					style = excel.CreateStyle();
                    style.Font.IsBold = true;
					style.Font.Size = 12;

					cells[currentUKRow - 2, 0].SetStyle(style);
					
					if((decimal)this.dataTable1.Rows[i][&quot;TotalSales&quot;] &gt; 5000)
					{
						cells[currentUKRow - 2, 3].PutValue(&quot;Exceeded Goal!&quot;);
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

					style = excel.GetNamedStyle(&quot;HeaderStyle&quot;);
					for(int j = 1; j &lt; 5; j++)
						cells[currentUKRow, (byte)j].SetStyle(style);
					cells[currentUKRow, 1].PutValue(&quot;Order ID:&quot;);
					cells[currentUKRow, 2].PutValue(&quot;Sales Amount:&quot;);
					cells[currentUKRow, 3].PutValue(&quot;Percent of Salesperson&apos;s Total:&quot;);
					cells[currentUKRow, 4].PutValue(&quot;Percent of Country Total:&quot;);
					currentUKRow ++;

					cells.ImportDataTable(dtSales[i], false, currentUKRow, 1);
					string startCellName1 = CellsHelper.CellIndexToName(currentUKRow, 2);
					string startCellName2 = CellsHelper.CellIndexToName(currentUKRow, 4);
					
					currentUKRow += dtSales[i].Rows.Count - 1;
					string endCellName1 = CellsHelper.CellIndexToName(currentUKRow, 2);
					string endCellName2 = CellsHelper.CellIndexToName(currentUKRow, 4);
					
					cells[currentUKRow + 1, 2].Formula = &quot;=sum(&quot; + startCellName1 + &quot;:&quot; 
						+ endCellName1 +&quot;)&quot;;

					cells[currentUKRow + 1, 4].Formula = &quot;=sum(&quot; + startCellName2 + &quot;:&quot; 
						+ endCellName2 +&quot;)&quot;;

					currentUKRow += 4;

				}
				else
				{
					sheet = excel.Worksheets[&quot;Employee Sales USA&quot;];
					cells = sheet.Cells;

					cells[currentUSARow - 2, 0].PutValue(&quot;Salesperson:&quot; + employeeName);

					style = excel.CreateStyle();
                    style.Font.IsBold = true;
					style.Font.Size = 12;
					cells[currentUSARow - 2, 0].SetStyle(style);
					
					if((decimal)this.dataTable1.Rows[i][&quot;TotalSales&quot;] &gt; 5000)
					{
						style = excel.CreateStyle();

                        cells[currentUSARow - 2, 3].PutValue(&quot;Exceeded Goal!&quot;);
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

					style = excel.GetNamedStyle(&quot;HeaderStyle&quot;);
					for(int j = 1; j &lt; 5; j++)
						cells[currentUSARow, (byte)j].SetStyle(style);
					cells[currentUSARow, 1].PutValue(&quot;Order ID:&quot;);
					cells[currentUSARow, 2].PutValue(&quot;Sales Amount:&quot;);
					cells[currentUSARow, 3].PutValue(&quot;Percent of Salesperson&apos;s Total:&quot;);
					cells[currentUSARow, 4].PutValue(&quot;Percent of Country Total:&quot;);
					currentUSARow ++;

					cells.ImportDataTable(dtSales[i], false, currentUSARow, 1);

					string startCellName1 = CellsHelper.CellIndexToName(currentUSARow, 2);
					string startCellName2 = CellsHelper.CellIndexToName(currentUSARow, 4);
					
					currentUSARow += dtSales[i].Rows.Count - 1;
					string endCellName1 = CellsHelper.CellIndexToName(currentUSARow, 2);
					string endCellName2 = CellsHelper.CellIndexToName(currentUSARow, 4);
					
					cells[currentUSARow + 1, 2].Formula = &quot;=sum(&quot; + startCellName1 + &quot;:&quot; 
						+ endCellName1 +&quot;)&quot;;

					cells[currentUSARow + 1, 4].Formula = &quot;=sum(&quot; + startCellName2 + &quot;:&quot; 
						+ endCellName2 +&quot;)&quot;;

					currentUSARow += 4;
				}
			}
			for(int i = 0; i &lt; excel.Worksheets.Count ; i ++)
			{
				sheet = excel.Worksheets[i];
				if(sheet.Name != &quot;Employee Sales UK&quot; &amp;&amp; sheet.Name != &quot;Employee Sales USA&quot;)
				{
					excel.Worksheets.RemoveAt(i);
					i --;
				}

			}
			excel.Save(destPath + &quot;EmployeeSales.xls&quot;);		
		}
```

### See Also

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


