---
title: WorksheetCollection.RemoveAt
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Removes the element at a specified name
type: docs
url: /net/aspose.cells/worksheetcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

Removes the element at a specified name.

```csharp
public void RemoveAt(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the element to remove. |

### Examples

```csharp
// Called: workbook.Worksheets.RemoveAt(&amp;quot;Sheet3&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet42954.xlsx&quot;);
            workbook.Worksheets.RemoveAt(&quot;Sheet3&quot;);
           Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;A1&quot;].Formula,&quot;=SUM(Sheet2:Sheet4!A1)&quot;);
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int) {#removeat}

Removes the element at a specified index.

```csharp
public void RemoveAt(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index value of the element to remove. |

### Examples

```csharp
// Called: excel.Worksheets.RemoveAt(i);
[Test]
		public void Method_Int32_()
		{
			
			Workbook excel = new Workbook();
			string designerFile = sourcePath + &quot;Northwind.xls&quot;;	
            excel = new Workbook(designerFile);

			this.dataTable1.Reset();
			this.oleDbSelectCommand1.CommandText = @&quot;SELECT [Order Subtotals].Subtotal, [Order Subtotals].OrderID, 
				Customers.CompanyName, Customers.CustomerID FROM Customers 
				INNER JOIN ([Order Subtotals] INNER JOIN Orders ON [Order Subtotals].OrderID = Orders.OrderID) 
				ON Customers.CustomerID = Orders.CustomerID 
				WHERE (Orders.ShippedDate BETWEEN #1/1/1995# AND #12/31/1995#) AND ([Order Subtotals].Subtotal &gt; 2500) 
				ORDER BY [Order Subtotals].Subtotal DESC&quot;;
			this.oleDbDataAdapter1.Fill(this.dataTable1);

			Worksheet sheet = excel.Worksheets[&quot;Sheet12&quot;];
			sheet.Name = &quot;Sales Totals&quot;;
			Cells cells = sheet.Cells;

			cells.ImportDataTable(this.dataTable1, false, 3, 1, this.dataTable1.Rows.Count, 3);

			decimal totalSum = 0.0m;
			for(int i = 0; i &lt; this.dataTable1.Rows.Count; i ++)
			{
				totalSum += (decimal)this.dataTable1.Rows[i][&quot;Subtotal&quot;];
				cells[3 + i, 5].PutValue( i + 1);
			}

			cells[3 + this.dataTable1.Rows.Count, 0].PutValue(&quot;Total:&quot;);
            Style style = excel.CreateStyle();
			style.Font.IsBold = true;
			cells[3 + this.dataTable1.Rows.Count, 0].SetStyle(style);

			cells[3 + this.dataTable1.Rows.Count, 1].PutValue((double)totalSum);
			
			for(int i = 0; i &lt; excel.Worksheets.Count ; i ++)
			{
				sheet = excel.Worksheets[i];
				if(sheet.Name != &quot;Sales Totals&quot;)
				{
					excel.Worksheets.RemoveAt(i);
					i --;
				}
			}
			
			excel.Save(destPath + &quot;SalesTotals.xls&quot;);		
		}
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


