---
title: Worksheet.AutoFitColumns
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Autofits all columns in this worksheet
type: docs
url: /net/aspose.cells/worksheet/autofitcolumns/
---
## AutoFitColumns() {#autofitcolumns}

Autofits all columns in this worksheet.

```csharp
public void AutoFitColumns()
```

### Examples

```csharp
// Called: workbook.Worksheets[0].AutoFitColumns();
public void Worksheet_Method_AutoFitColumns()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    workbook.Worksheets[0].AutoFitColumns();
    int w = workbook.Worksheets[0].Cells.GetColumnWidthPixel(0);
    Assert.IsTrue(w == 61 || w == 63 || w == 56);
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(AutoFitterOptions) {#autofitcolumns_1}

Autofits all columns in this worksheet.

```csharp
public void AutoFitColumns(AutoFitterOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | AutoFitterOptions | The auto fitting options |

### Examples

```csharp
// Called: workbook.Worksheets[1].AutoFitColumns(options);
public void Worksheet_Method_AutoFitColumns()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    AutoFitterOptions options = new AutoFitterOptions();
    //   options.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
    workbook.Worksheets[1].AutoFitColumns(options);
    Cells cells = workbook.Worksheets[1].Cells;

    int w = cells.GetColumnWidthPixel(14 + 0);
    Assert.IsTrue(w == 48 || w==42 );
    w = cells.GetColumnWidthPixel(14 + 1);
    Assert.IsTrue(w == 27 || w == 29);
    w = cells.GetColumnWidthPixel(14 + 2);
    Assert.IsTrue(w == 41 || w == 36);
    workbook.Save(Constants.destPath  + "example.xlsx");

}
```

### See Also

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int) {#autofitcolumns_2}

Autofits the columns width.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | Int32 | First column index. |
| lastColumn | Int32 | Last column index. |

### Remarks

AutoFitColumn is an imprecise function.

### Examples

```csharp
// Called: sheet.AutoFitColumns(0, 3);
public void Worksheet_Method_AutoFitColumns()
{
    Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xlsx");
    Aspose.Cells.Worksheet sheet = workbook.Worksheets[0];

    sheet.AutoFitColumns(0, 3);
    Assert.AreEqual(79, sheet.Cells.GetColumnWidthPixel(0));
    Assert.AreEqual(184, sheet.Cells.GetColumnWidthPixel(1));
    Assert.AreEqual(100, sheet.Cells.GetColumnWidthPixel(2));
    Assert.AreEqual(1822, sheet.Cells.GetColumnWidthPixel(3));
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, AutoFitterOptions) {#autofitcolumns_3}

Autofits the columns width.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | Int32 | First column index. |
| lastColumn | Int32 | Last column index. |
| options | AutoFitterOptions | The auto fitting options |

### Remarks

AutoFitColumn is an imprecise function.

### Examples

```csharp
namespace AsposeCellsExamples.WorksheetMethodAutoFitColumnsWithInt32Int32AutoFitterOptionsDemo
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnsWithInt32Int32AutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to cells
            worksheet.Cells["A1"].PutValue("Short text");
            worksheet.Cells["B1"].PutValue("This is a much longer text that needs column autofitting");
            worksheet.Cells["C1"].PutValue("Another example with different length");

            // Create AutoFitterOptions with specific settings
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;
            options.IgnoreHidden = false;
            options.OnlyAuto = false;

            try
            {
                // Call AutoFitColumns with parameters (firstColumn, lastColumn, options)
                worksheet.AutoFitColumns(0, 2, options);
                
                Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, AutoFitterOptions)");
                
                // Display the effect by showing column widths
                Console.WriteLine($"Column A width: {worksheet.Cells.GetColumnWidth(0)}");
                Console.WriteLine($"Column B width: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine($"Column C width: {worksheet.Cells.GetColumnWidth(2)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### See Also

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, int, int) {#autofitcolumns_4}

Autofits the columns width.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row index. |
| firstColumn | Int32 | First column index. |
| lastRow | Int32 | Last row index. |
| lastColumn | Int32 | Last column index. |

### Remarks

AutoFitColumn is an imprecise function.

### Examples

```csharp
// Called: worksheet.AutoFitColumns(18, 3, 78, 52);
public void Worksheet_Method_AutoFitColumns()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];
    worksheet.AutoFitColumns(18, 3, 78, 52);
    Assert.AreEqual(64,worksheet.Cells.GetColumnWidthPixel(3));
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, int, int, AutoFitterOptions) {#autofitcolumns_5}

Autofits the columns width.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, 
    AutoFitterOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row index. |
| firstColumn | Int32 | First column index. |
| lastRow | Int32 | Last row index. |
| lastColumn | Int32 | Last column index. |
| options | AutoFitterOptions | The auto fitting options |

### Remarks

AutoFitColumn is an imprecise function.

### Examples

```csharp
namespace AsposeCellsExamples.WorksheetMethodAutoFitColumnsWithInt32Int32Int32Int32AutoFitterDemo
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnsWithInt32Int32Int32Int32AutoFitterDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate cells with sample data that needs column width adjustment
            worksheet.Cells["A1"].PutValue("This is a long text that needs column autofit");
            worksheet.Cells["B1"].PutValue("Another lengthy text string for demonstration");
            worksheet.Cells["C1"].PutValue("Short");
            worksheet.Cells["A2"].PutValue(12345.6789);
            worksheet.Cells["B2"].PutValue("Multi-line\ntext\nsample");
            worksheet.Cells["C2"].PutValue(true);

            // Create AutoFitterOptions with specific settings
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;
            options.IgnoreHidden = false;
            options.OnlyAuto = false;

            try
            {
                // Call AutoFitColumns with specific parameters (firstRow, firstColumn, lastRow, lastColumn, options)
                worksheet.AutoFitColumns(0, 0, 1, 2, options);
                
                Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, Int32, Int32, AutoFitterOptions)");
                
                // Display column widths after autofit
                Console.WriteLine($"Column A width after autofit: {worksheet.Cells.GetColumnWidth(0)}");
                Console.WriteLine($"Column B width after autofit: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine($"Column C width after autofit: {worksheet.Cells.GetColumnWidth(2)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### See Also

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


