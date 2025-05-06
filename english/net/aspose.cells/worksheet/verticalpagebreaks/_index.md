---
title: Worksheet.VerticalPageBreaks
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the VerticalPageBreakCollection collection
type: docs
url: /net/aspose.cells/worksheet/verticalpagebreaks/
---
## Worksheet.VerticalPageBreaks property

Gets the [`VerticalPageBreakCollection`](../../verticalpagebreakcollection/) collection.

```csharp
public VerticalPageBreakCollection VerticalPageBreaks { get; }
```

### Examples

```csharp
// Called: VerticalPageBreakCollection vPageBreaks = sheet.VerticalPageBreaks;
[Test]
		public void Property_VerticalPageBreaks()
		{
			
			Workbook excel = new Workbook();
			string designerFile = sourcePath + &quot;Northwind.xls&quot;;	
            excel = new Workbook(designerFile);
			
			this.dataTable1.Reset();
			this.oleDbDataAdapter1.SelectCommand.CommandText = @&quot;SELECT DISTINCTROW Categories.CategoryID, 
					Categories.CategoryName, Products.ProductName, SUM([Order Details Extended].ExtendedPrice) AS ProductSales
				FROM  Categories 
				INNER JOIN
					(Products INNER JOIN (Orders INNER JOIN [Order Details Extended] ON
					Orders.OrderID = [Order Details Extended].OrderID) ON Products.ProductID = [Order Details Extended].ProductID) ON Categories.CategoryID = Products.CategoryID
				WHERE
					(((Orders.OrderDate) BETWEEN #1/1/1995# AND #12/31/1995#)) GROUP BY Categories.CategoryID ,  Categories.CategoryName ,  Products.ProductName ORDER BY Categories.CategoryName&quot;;
			this.oleDbDataAdapter1.Fill(this.dataTable1);
			
			Worksheet sheet = excel.Worksheets[&quot;Sheet8&quot;];
			sheet.Name = &quot;Sales By Category&quot;;
			Cells cells = sheet.Cells;
			VerticalPageBreakCollection vPageBreaks = sheet.VerticalPageBreaks;
			int currentRow = 2;
			byte currentColumn = 0;

			string lastCategory = &quot;&quot;;
			string thisCategory, nextCategory;

			SetSalesByCategoryStyles(excel);
			for(int i = 0; i &lt; this.dataTable1.Rows.Count; i ++)
			{
				thisCategory = (string)this.dataTable1.Rows[i][&quot;CategoryName&quot;];
				if(thisCategory != lastCategory)
				{
					currentRow = 2;
					if(i != 0)
						currentColumn += 15;
					CreateSalesByCategoryHeader(excel, cells, currentRow, currentColumn,thisCategory);
					lastCategory = thisCategory;
					currentRow += 2;
				}
				cells[currentRow, currentColumn].PutValue((string)this.dataTable1.Rows[i][&quot;ProductName&quot;]);
				cells[currentRow, (byte)(currentColumn + 1)].PutValue((double)(decimal)this.dataTable1.Rows[i][&quot;ProductSales&quot;]);

				cells[currentRow, (byte)(currentColumn + 1)].SetStyle(excel.GetNamedStyle(&quot;Sales&quot;));

				cells.SetColumnWidth(currentColumn, 27);
				cells.SetColumnWidth((byte)(currentColumn + 1), 15);

				if( i != this.dataTable1.Rows.Count - 1)
				{
					nextCategory = (string)this.dataTable1.Rows[i + 1][&quot;CategoryName&quot;];
					if(thisCategory != nextCategory)
					{
						vPageBreaks.Add(0, currentColumn + 1);
						CreateChart(excel, sheet, currentRow, currentColumn);
					}
				}
				else
				{
					CreateChart(excel, sheet, currentRow, currentColumn);
				}
				currentRow ++;
			}
			for(int i = 0; i &lt; excel.Worksheets.Count ; i ++)
			{
				sheet = excel.Worksheets[i];
				if(sheet.Name != &quot;Sales By Category&quot;)
				{
					excel.Worksheets.RemoveAt(i);
					i --;
				}
			}
			excel.Save(destPath + &quot;SalesByCategory.xls&quot;);		
		}
```

### See Also

* class [VerticalPageBreakCollection](../../verticalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


