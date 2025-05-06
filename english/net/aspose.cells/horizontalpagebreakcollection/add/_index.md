---
title: HorizontalPageBreakCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: HorizontalPageBreakCollection method. Adds a horizontal page break to the collection
type: docs
url: /net/aspose.cells/horizontalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Adds a horizontal page break to the collection.

```csharp
public int Add(int row, int startColumn, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index, zero based. |
| startColumn | Int32 | Start column index, zero based. |
| endColumn | Int32 | End column index, zero based. |

### Return Value

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Remarks

This method is used to add a horizontal pagebreak within a print area.

### Examples

```csharp
// Called: worksheet.HorizontalPageBreaks.Add(10, 1, 5);
public static void Method_Int32_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add a horizontal page break at row 5
            worksheet.HorizontalPageBreaks.Add(5);
            
            // Add a horizontal page break at row 10, starting from column 1 to column 5
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            // Add a horizontal page break at row 15, starting from column 2
            worksheet.HorizontalPageBreaks.Add(15, 2);
            
            // Add a horizontal page break at cell &quot;G5&quot;
            worksheet.HorizontalPageBreaks.Add(&quot;G5&quot;);
            
            // Remove the first horizontal page break
            worksheet.HorizontalPageBreaks.RemoveAt(0);
            
            // Save the workbook
            workbook.Save(&quot;HorizontalPageBreakCollectionExample.xlsx&quot;);
            workbook.Save(&quot;HorizontalPageBreakCollectionExample.pdf&quot;);
            return;
        }
```

### See Also

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Adds a horizontal page break to the collection.

```csharp
public int Add(int row)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Cell row index, zero based. |

### Return Value

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Remarks

Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

### Examples

```csharp
// Called: worksheet.HorizontalPageBreaks.Add(5);
public static void Method_Int32_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add a horizontal page break at row 5
            worksheet.HorizontalPageBreaks.Add(5);
            
            // Add a horizontal page break at row 10, starting from column 1 to column 5
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            // Add a horizontal page break at row 15, starting from column 2
            worksheet.HorizontalPageBreaks.Add(15, 2);
            
            // Add a horizontal page break at cell &quot;G5&quot;
            worksheet.HorizontalPageBreaks.Add(&quot;G5&quot;);
            
            // Remove the first horizontal page break
            worksheet.HorizontalPageBreaks.RemoveAt(0);
            
            // Save the workbook
            workbook.Save(&quot;HorizontalPageBreakCollectionExample.xlsx&quot;);
            workbook.Save(&quot;HorizontalPageBreakCollectionExample.pdf&quot;);
            return;
        }
```

### See Also

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Adds a horizontal page break to the collection.

```csharp
public int Add(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Cell row index, zero based. |
| column | Int32 | Cell column index, zero based. |

### Return Value

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Remarks

Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

### Examples

```csharp
// Called: hPageBreaks.Add(currentRow, 0);
[Test]
		public void Method_Int32_()
		{
			Workbook excel = new Workbook();
			string designerFile = sourcePath + &quot;Northwind.xls&quot;;
			
            excel = new Workbook(designerFile);
			
			ReadCategory();
			DataTable dataTable2 = new DataTable();
			
			Worksheet sheet = excel.Worksheets[&quot;Sheet2&quot;];
			sheet.Name = &quot;Catalog&quot;;
			Cells cells = sheet.Cells;

			int currentRow = 55;

			//Add LightGray color to color palette
			excel.ChangePalette(Color.LightGray, 55);


            //Set CategoryName style

            Style styleCategoryName = excel.CreateStyle();

            styleCategoryName.Font.Size = 14;
			styleCategoryName.Font.Color = Color.Blue;
			styleCategoryName.Font.IsBold = true;
			styleCategoryName.Font.Name = &quot;Times New Roman&quot;;

	
			Style styleDescription = excel.CreateStyle();
            styleDescription.Font.Name = &quot;Times New Roman&quot;;
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
            styleNumber.Font.Name = &quot;Times New Roman&quot;;
			styleNumber.Number = 8;


            HorizontalPageBreakCollection hPageBreaks = sheet.HorizontalPageBreaks;
			
			string cmdText = &quot;SELECT ProductName, ProductID, QuantityPerUnit, &quot; +
				&quot;UnitPrice FROM Products&quot;;
			for(int i = 0; i &lt; this.dataTable1.Rows.Count; i ++)
			{
				currentRow += 2;
				cells.SetRowHeight(currentRow, 20);
				cells[currentRow, 1].SetStyle(styleCategoryName);
				DataRow categoriesRow = this.dataTable1.Rows[i];
				
				//Write CategoryName
				cells[currentRow, 1].PutValue((string)categoriesRow[&quot;CategoryName&quot;]);

				//Write Description
				currentRow ++;
				cells[currentRow, 1].PutValue((string)categoriesRow[&quot;Description&quot;]);
				cells[currentRow, 1].SetStyle(styleDescription);

				dataTable2.Clear();
				oleDbDataAdapter2.SelectCommand.CommandText = cmdText +&quot; where categoryid = &quot; 
					+ categoriesRow[&quot;CategoryID&quot;].ToString();
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

			for(int i = 0; i &lt; excel.Worksheets.Count ; i ++)
			{
				sheet = excel.Worksheets[i];
				if(sheet.Name != &quot;Catalog&quot;)
				{
					excel.Worksheets.RemoveAt(i);
					i --;
				}

			}
			excel.Save(destPath + &quot;Catalog.xls&quot;);
		}
```

### See Also

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Adds a horizontal page break to the collection.

```csharp
public int Add(string cellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |

### Return Value

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Remarks

Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.

### Examples

```csharp
// Called: workbook.Worksheets[0].HorizontalPageBreaks.Add(&amp;quot;D5&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Test_125861.XLS&quot;);
            workbook.Worksheets[0].HorizontalPageBreaks.Add(&quot;D5&quot;);
            workbook.Save(Constants.destPath + &quot;Test_125861.xls&quot;);
        }
```

### See Also

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


