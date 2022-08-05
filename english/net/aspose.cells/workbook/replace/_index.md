---
title: Replace
second_title: Aspose.Cells for .NET API Reference
description: Replaces a cells value with a new string.
type: docs
weight: 590
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

* class [Workbook](../../workbook)
* namespace [Aspose.Cells](../../workbook)
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

* class [Workbook](../../workbook)
* namespace [Aspose.Cells](../../workbook)
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

* class [Workbook](../../workbook)
* namespace [Aspose.Cells](../../workbook)
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

* class [Workbook](../../workbook)
* namespace [Aspose.Cells](../../workbook)
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

* class [Workbook](../../workbook)
* namespace [Aspose.Cells](../../workbook)
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

* class [Workbook](../../workbook)
* namespace [Aspose.Cells](../../workbook)
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

* class [Workbook](../../workbook)
* namespace [Aspose.Cells](../../workbook)
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

### See Also

* class [Workbook](../../workbook)
* namespace [Aspose.Cells](../../workbook)
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

### See Also

* class [Workbook](../../workbook)
* namespace [Aspose.Cells](../../workbook)
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

### See Also

* class [ReplaceOptions](../../replaceoptions)
* class [Workbook](../../workbook)
* namespace [Aspose.Cells](../../workbook)
* assembly [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
