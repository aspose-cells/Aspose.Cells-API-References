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
public static void HorizontalPageBreakCollection_Method_Add()
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
            
            // Add a horizontal page break at cell "G5"
            worksheet.HorizontalPageBreaks.Add("G5");
            
            // Remove the first horizontal page break
            worksheet.HorizontalPageBreaks.RemoveAt(0);
            
            // Save the workbook
            workbook.Save("HorizontalPageBreakCollectionExample.xlsx");
            workbook.Save("HorizontalPageBreakCollectionExample.pdf");
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
public static void HorizontalPageBreakCollection_Method_Add()
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
            
            // Add a horizontal page break at cell "G5"
            worksheet.HorizontalPageBreaks.Add("G5");
            
            // Remove the first horizontal page break
            worksheet.HorizontalPageBreaks.RemoveAt(0);
            
            // Save the workbook
            workbook.Save("HorizontalPageBreakCollectionExample.xlsx");
            workbook.Save("HorizontalPageBreakCollectionExample.pdf");
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
// Called: sheet.HorizontalPageBreaks.Add(startRow - 1, 0);
		public void HorizontalPageBreakCollection_Method_Add()
		{
			Workbook excel = new Workbook();
			this.dataTable1.Reset();
			this.oleDbDataAdapter1.SelectCommand.CommandText = "SELECT OrderID FROM Orders ORDER BY OrderID DESC";
			this.oleDbDataAdapter1.Fill(this.dataTable1);

			DataTable[] dtInvoice = new DataTable[this.dataTable1.Rows.Count];
			
			for(int i = 0; i < dtInvoice.Length; i ++)
				dtInvoice[i] = this.ReadInvoice(this.dataTable1.Rows[i][0].ToString());
			
			
			WorksheetCollection sheets = excel.Worksheets;
			Worksheet sheet = sheets[0];
			sheet.Name = "Invoice";

			Cells cells = sheet.Cells;
			int startRow = 0;
	
			SetInvoiceStyles(excel);
			for(int i = 0; i < dtInvoice.Length; i ++)
			{
				
						
				sheet.Pictures.Add(startRow, 0, startRow + 2, 1, sourcePath + "Image\\logo.jpg");
				int picIndex = sheet.Pictures.Add(startRow, 1, startRow + 2, 2, sourcePath + "Image\\namelogo.jpg");
				Picture pic = sheet.Pictures[picIndex];
				pic.UpperDeltaY = 100;
				
				CreateInvoiceHeader(cells, excel, dtInvoice[i], startRow);
				startRow += 11;
				CreateOrder(cells, excel, dtInvoice[i], startRow, this.dataTable1.Rows[i][0].ToString());
				startRow += 4;
				CreateOrderDetail(cells, excel, dtInvoice[i], startRow);

				startRow += dtInvoice[i].Rows.Count + 1;
				sheet.HorizontalPageBreaks.Add(startRow - 1, 0);
			}

			excel.Save(destPath + "Invoice.xls");		

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
// Called: workbook.Worksheets[0].HorizontalPageBreaks.Add("D5");
public void HorizontalPageBreakCollection_Method_Add()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "Test_125861.XLS");
    workbook.Worksheets[0].HorizontalPageBreaks.Add("D5");
    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


