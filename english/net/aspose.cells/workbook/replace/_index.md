---
title: Workbook.Replace
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Replaces a cells value with a new string
type: docs
url: /net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

Replaces a cell's value with a new string.

```csharp
public int Replace(string placeHolder, string newValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | String | String value to replace |

### Examples

```csharp
[C#]

Workbook workbook = new Workbook();
//......
workbook.Replace("AnOldValue", "NewValue");

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
'........
workbook.Replace("AnOldValue", "NewValue")
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

Replaces a cell's value with a new integer.

```csharp
public int Replace(string placeHolder, int newValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | Int32 | Integer value to replace |

### Examples

```csharp
[C#]

Workbook workbook = new Workbook();
//......
int newValue = 100;
workbook.Replace("AnOldValue", newValue);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
'.........
Dim NewValue As Integer =  100 
workbook.Replace("AnOldValue", NewValue)
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

Replaces a cell's value with a new double.

```csharp
public int Replace(string placeHolder, double newValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | Double | Double value to replace |

### Examples

```csharp

[C#]

Workbook workbook = new Workbook();
//......
double newValue = 100.0;
workbook.Replace("AnOldValue", newValue);


[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
'.........
Dim NewValue As Double =  100.0
workbook.Replace("AnOldValue", NewValue)
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

Replaces a cell's value with a new string array.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValues | String[] | String array to replace |
| isVertical | Boolean | True - Vertical, False - Horizontal |

### Examples

```csharp

[C#]

Workbook workbook = new Workbook();
//......
string[] newValues = new string[]{"Tom", "Alice", "Jerry"};
workbook.Replace("AnOldValue", newValues, true);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
'.............
Dim NewValues() As String =  New String() {"Tom", "Alice", "Jerry"}		
workbook.Replace("AnOldValue", NewValues, True)
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

Replaces cells' values with an integer array.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValues | Int32[] | Integer array to replace |
| isVertical | Boolean | True - Vertical, False - Horizontal |

### Examples

```csharp
[C#]

Workbook workbook = new Workbook();
//......
int[] newValues = new int[]{1, 2, 3};
workbook.Replace("AnOldValue", newValues, true);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
'...........
Dim NewValues() As Integer =  New Integer() {1, 2, 3}
workbook.Replace("AnOldValue", NewValues, True)
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

Replaces cells' values with a double array.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValues | Double[] | Double array to replace |
| isVertical | Boolean | True - Vertical, False - Horizontal |

### Examples

```csharp

[C#]

Workbook workbook = new Workbook();
//......
double[] newValues = new double[]{1.23, 2.56, 3.14159};
workbook.Replace("AnOldValue", newValues, true);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
'...........
Dim NewValues() As Double =  New Double() {1.23, 2.56, 3.14159}
workbook.Replace("AnOldValue", NewValues, True)
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

Replaces cells' values with data from a DataTable.

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| insertTable | DataTable | DataTable to replace |

### Examples

```csharp
[C#]

Workbook workbook = new Workbook();
DataTable myDataTable = new DataTable("Customers");
// Adds data to myDataTable
//........
workbook.Replace("AnOldValue", myDataTable);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
Dim myDataTable As DataTable =  New DataTable("Customers") 
' Adds data to myDataTable
'.............
workbook.Replace("AnOldValue", myDataTable)
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

Replaces cells' values with new data.

```csharp
public int Replace(bool boolValue, object newValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| boolValue | Boolean | The boolean value to be replaced. |
| newValue | Object | New value. Can be string, integer, double or DateTime value. |

### Examples

```csharp
namespace AsposeCellsExamples.WorkbookMethodReplaceWithBooleanObjectDemo
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithBooleanObjectDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Populate some cells with boolean values
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            worksheet.Cells["A3"].PutValue(true);
            
            try
            {
                // Call the Replace method to replace all 'true' values with "REPLACED"
                int replacements = workbook.Replace(true, "REPLACED");
                
                Console.WriteLine($"Replaced {replacements} occurrences of 'true' with 'REPLACED'");
                
                // Display the results
                Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("WorkbookMethodReplaceWithBooleanObjectDemo.xlsx");
        }
    }
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

Replaces cells' values with new data.

```csharp
public int Replace(int intValue, object newValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| intValue | Int32 | The integer value to be replaced. |
| newValue | Object | New value. Can be string, integer, double or DateTime value. |

### Examples

```csharp
namespace AsposeCellsExamples.WorkbookMethodReplaceWithInt32ObjectDemo
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithInt32ObjectDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Populate some cells with integer values to be replaced
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(100);
            
            try
            {
                // Call the Replace method with parameters (Int32, Object)
                int replacements = workbook.Replace(100, "ReplacedValue");
                
                Console.WriteLine($"Replaced {replacements} occurrences of the value 100");
                
                // Display the worksheet content after replacement
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("WorkbookMethodReplaceWithInt32ObjectDemo.xlsx");
        }
    }
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

Replaces a cell's value with a new string.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | String | String value to replace |
| options | ReplaceOptions | The replace options |

### Examples

```csharp
// Called: int replacedCount = workbook.Replace("Hello", "Hi", options);
public static void Workbook_Method_Replace()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data to the worksheet
            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            // Create ReplaceOptions
            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false,
                RegexKey = false
            };

            // Replace "Hello" with "Hi" in the worksheet
            int replacedCount = workbook.Replace("Hello", "Hi", options);

            // Output the number of replacements made
            Console.WriteLine($"Number of replacements made: {replacedCount}");

            // Save the workbook
            workbook.Save("ReplaceOptionsExample.xlsx");
        }
```

### See Also

* class [ReplaceOptions](../../replaceoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


