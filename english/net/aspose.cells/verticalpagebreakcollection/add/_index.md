---
title: VerticalPageBreakCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: VerticalPageBreakCollection method. Adds a vertical page break to the collection
type: docs
url: /net/aspose.cells/verticalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Adds a vertical page break to the collection.

```csharp
public int Add(int startRow, int endRow, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index, zero based. |
| endRow | Int32 | End row index, zero based. |
| column | Int32 | Column index, zero based. |

### Return Value

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Remarks

This method is used to add a vertical pagebreak within a print area.

### Examples

```csharp
// Called: verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
public static void Method_Int32_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the VerticalPageBreakCollection of the worksheet
            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Add vertical page breaks
            verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
            verticalPageBreaks.Add(4); // At column 4
            verticalPageBreaks.Add(5, 3); // At row 5, column 3
            verticalPageBreaks.Add(&quot;G5&quot;); // At cell G5

            // Remove a vertical page break at index 1
            verticalPageBreaks.RemoveAt(1);

            // Access and print details of the vertical page breaks
            for (int i = 0; i &lt; verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($&quot;Vertical Page Break {i}: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}&quot;);
            }

            // Save the workbook
            workbook.Save(&quot;VerticalPageBreakCollectionExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Adds a vertical page break to the collection.

```csharp
public int Add(int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Cell column index, zero based. |

### Return Value

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Remarks

Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

### Examples

```csharp
// Called: verticalPageBreaks.Add(4); // At column 4
public static void Method_Int32_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the VerticalPageBreakCollection of the worksheet
            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Add vertical page breaks
            verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
            verticalPageBreaks.Add(4); // At column 4
            verticalPageBreaks.Add(5, 3); // At row 5, column 3
            verticalPageBreaks.Add(&quot;G5&quot;); // At cell G5

            // Remove a vertical page break at index 1
            verticalPageBreaks.RemoveAt(1);

            // Access and print details of the vertical page breaks
            for (int i = 0; i &lt; verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($&quot;Vertical Page Break {i}: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}&quot;);
            }

            // Save the workbook
            workbook.Save(&quot;VerticalPageBreakCollectionExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Adds a vertical page break to the collection.

```csharp
public int Add(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Cell row index, zero based. |
| column | Int32 | Cell column index, zero based. |

### Return Value

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Remarks

Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

### Examples

```csharp
// Called: vPageBreaks.Add(0, currentColumn + 1);
[Test]
		public void Method_Int32_()
		{
			
			Workbook excel = new Workbook();
			string designerFile = sourcePath + &quot;Northwind.xls&quot;;
            excel = new Workbook(designerFile);
			
			this.dataTable1.Reset();
			this.oleDbDataAdapter1.SelectCommand.CommandText =@&quot;SELECT Categories.CategoryName, Products.ProductName, Products.QuantityPerUnit, Products.UnitsInStock, Products.Discontinued, Categories.CategoryID, Products.ProductID FROM Categories INNER JOIN Products ON Categories.CategoryID = Products.CategoryID WHERE (Products.Discontinued &lt;&gt; Yes) ORDER BY Categories.CategoryName, Products.ProductName&quot;;
			this.oleDbDataAdapter1.Fill(this.dataTable1);
		
			Worksheet sheet = excel.Worksheets[&quot;Sheet7&quot;];
			sheet.Name = &quot;Products By Category&quot;;
			Cells cells = sheet.Cells;
			VerticalPageBreakCollection vPageBreaks = sheet.VerticalPageBreaks;
			cells.SetRowHeight(4, 20.25);
			cells.SetRowHeight(5, 18.75);
			ushort currentRow = 4;
			byte currentColumn = 0;

			string lastCategory = &quot;&quot;;
			string thisCategory, nextCategory;

			int productsCount = 0;

			SetProductsByCategoryStyles(excel);
			for(int i = 0; i &lt; this.dataTable1.Rows.Count; i ++)
			{
				thisCategory = (string)this.dataTable1.Rows[i][&quot;CategoryName&quot;];
				if(thisCategory != lastCategory)
				{
					currentRow = 4;
					if(i != 0)
						currentColumn += 4;
					CreateProductsByCategoryHeader(excel, cells, currentRow, currentColumn, thisCategory);
					lastCategory = thisCategory;
					currentRow += 2;
				}
				cells[currentRow, currentColumn].PutValue((string)this.dataTable1.Rows[i][&quot;ProductName&quot;]);
				cells[currentRow, (byte)(currentColumn + 1)].PutValue((short)this.dataTable1.Rows[i][&quot;UnitsInStock&quot;]);

				if( i != this.dataTable1.Rows.Count - 1)
				{
					nextCategory = (string)this.dataTable1.Rows[i + 1][&quot;CategoryName&quot;];
					if(thisCategory != nextCategory)
					{
						Style style = excel.GetNamedStyle(&quot;ProductsCount&quot;);
						cells[currentRow + 1, currentColumn].PutValue(&quot;Number of Products:&quot;);
						cells[currentRow + 1, currentColumn].SetStyle(style);
						
						style = excel.GetNamedStyle(&quot;CountNumber&quot;);
						cells[currentRow + 1, (byte)(currentColumn + 1)].PutValue(productsCount + 1);
						cells[currentRow + 1, (byte)(currentColumn + 1)].SetStyle(style);
						currentRow ++;
						productsCount = 0;
						vPageBreaks.Add(0, currentColumn + 1);
					}
					else
						productsCount ++;
				}
				else
				{
					Style style = excel.GetNamedStyle(&quot;ProductsCount&quot;);
					cells[currentRow + 1, currentColumn].PutValue(&quot;Number of Products:&quot;);
					cells[currentRow + 1, currentColumn].SetStyle(style);
						
					style = excel.GetNamedStyle(&quot;CountNumber&quot;);
					cells[currentRow + 1, (byte)(currentColumn + 1)].PutValue(productsCount + 1);
					cells[currentRow + 1, (byte)(currentColumn + 1)].SetStyle(style);
				}
				currentRow ++;
			}

			for(int i = 0; i &lt; excel.Worksheets.Count ; i ++)
			{
				sheet = excel.Worksheets[i];
				if(sheet.Name != &quot;Products By Category&quot;)
				{
					excel.Worksheets.RemoveAt(i);
					i --;
				}
			}

			excel.Save(destPath + &quot;ProductsByCategory.xls&quot;);		
		}
```

### See Also

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Adds a vertical page break to the collection.

```csharp
public int Add(string cellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |

### Return Value

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Remarks

Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

### Examples

```csharp
// Called: worksheet.VerticalPageBreaks.Add(&amp;quot;G5&amp;quot;);
public static void Method_String_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet in the workbook
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add a vertical page break at column G (index 6)
            worksheet.VerticalPageBreaks.Add(&quot;G5&quot;);

            // Save the workbook
            workbook.Save(&quot;VerticalPageBreakExample.xlsx&quot;);

            // Access the added vertical page break
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];

            // Display the properties of the vertical page break
            Console.WriteLine(&quot;Start Row: &quot; + vpb.StartRow);
            Console.WriteLine(&quot;End Row: &quot; + vpb.EndRow);
            Console.WriteLine(&quot;Column: &quot; + vpb.Column);
        }
```

### See Also

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


