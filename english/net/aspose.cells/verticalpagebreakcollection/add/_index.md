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
            verticalPageBreaks.Add("G5"); // At cell G5

            // Remove a vertical page break at index 1
            verticalPageBreaks.RemoveAt(1);

            // Access and print details of the vertical page breaks
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"Vertical Page Break {i}: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");
            }

            // Save the workbook
            workbook.Save("VerticalPageBreakCollectionExample.xlsx");

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
            verticalPageBreaks.Add("G5"); // At cell G5

            // Remove a vertical page break at index 1
            verticalPageBreaks.RemoveAt(1);

            // Access and print details of the vertical page breaks
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"Vertical Page Break {i}: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");
            }

            // Save the workbook
            workbook.Save("VerticalPageBreakCollectionExample.xlsx");

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
			string designerFile = sourcePath + "Northwind.xls";	
            excel = new Workbook(designerFile);
			
			this.dataTable1.Reset();
			this.oleDbDataAdapter1.SelectCommand.CommandText = @"SELECT DISTINCTROW Categories.CategoryID, 
					Categories.CategoryName, Products.ProductName, SUM([Order Details Extended].ExtendedPrice) AS ProductSales
				FROM  Categories 
				INNER JOIN
					(Products INNER JOIN (Orders INNER JOIN [Order Details Extended] ON
					Orders.OrderID = [Order Details Extended].OrderID) ON Products.ProductID = [Order Details Extended].ProductID) ON Categories.CategoryID = Products.CategoryID
				WHERE
					(((Orders.OrderDate) BETWEEN #1/1/1995# AND #12/31/1995#)) GROUP BY Categories.CategoryID ,  Categories.CategoryName ,  Products.ProductName ORDER BY Categories.CategoryName";
			this.oleDbDataAdapter1.Fill(this.dataTable1);
			
			Worksheet sheet = excel.Worksheets["Sheet8"];
			sheet.Name = "Sales By Category";
			Cells cells = sheet.Cells;
			VerticalPageBreakCollection vPageBreaks = sheet.VerticalPageBreaks;
			int currentRow = 2;
			byte currentColumn = 0;

			string lastCategory = "";
			string thisCategory, nextCategory;

			SetSalesByCategoryStyles(excel);
			for(int i = 0; i < this.dataTable1.Rows.Count; i ++)
			{
				thisCategory = (string)this.dataTable1.Rows[i]["CategoryName"];
				if(thisCategory != lastCategory)
				{
					currentRow = 2;
					if(i != 0)
						currentColumn += 15;
					CreateSalesByCategoryHeader(excel, cells, currentRow, currentColumn,thisCategory);
					lastCategory = thisCategory;
					currentRow += 2;
				}
				cells[currentRow, currentColumn].PutValue((string)this.dataTable1.Rows[i]["ProductName"]);
				cells[currentRow, (byte)(currentColumn + 1)].PutValue((double)(decimal)this.dataTable1.Rows[i]["ProductSales"]);

				cells[currentRow, (byte)(currentColumn + 1)].SetStyle(excel.GetNamedStyle("Sales"));

				cells.SetColumnWidth(currentColumn, 27);
				cells.SetColumnWidth((byte)(currentColumn + 1), 15);

				if( i != this.dataTable1.Rows.Count - 1)
				{
					nextCategory = (string)this.dataTable1.Rows[i + 1]["CategoryName"];
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
			for(int i = 0; i < excel.Worksheets.Count ; i ++)
			{
				sheet = excel.Worksheets[i];
				if(sheet.Name != "Sales By Category")
				{
					excel.Worksheets.RemoveAt(i);
					i --;
				}
			}
			excel.Save(destPath + "SalesByCategory.xls");		
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
// Called: worksheet.VerticalPageBreaks.Add("G5");
public static void Method_String_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet in the workbook
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add a vertical page break at column G (index 6)
            worksheet.VerticalPageBreaks.Add("G5");

            // Save the workbook
            workbook.Save("VerticalPageBreakExample.xlsx");

            // Access the added vertical page break
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];

            // Display the properties of the vertical page break
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
```

### See Also

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


