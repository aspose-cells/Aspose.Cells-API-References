---
title: Replace
second_title: Aspose.Cells for .NET API 参考
description: 将单元格的值替换为新字符串
type: docs
weight: 570
url: /zh/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

将单元格的值替换为新字符串。

```csharp
public int Replace(string placeHolder, string newValue)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | String | 单元格占位符 |
| newValue | String | 要替换的字符串值 |

### 例子

```csharp
[C#]

Workbook workbook = new Workbook();
......
workbook.Replace("AnOldValue", "NewValue");

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
 ........
orkbook.Replace("AnOldValue", "NewValue")
```

### 也可以看看

* class [Workbook](../../workbook)
* 命名空间 [Aspose.Cells](../../workbook)
* 部件 [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

将单元格的值替换为新整数。

```csharp
public int Replace(string placeHolder, int newValue)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | String | 单元格占位符 |
| newValue | Int32 | 要替换的整数值 |

### 例子

```csharp
[C#]

Workbook workbook = new Workbook();
......
int newValue = 100;
workbook.Replace("AnOldValue", newValue);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
........
im NewValue As Integer =  100 
orkbook.Replace("AnOldValue", NewValue)
```

### 也可以看看

* class [Workbook](../../workbook)
* 命名空间 [Aspose.Cells](../../workbook)
* 部件 [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

将单元格的值替换为新的双精度值。

```csharp
public int Replace(string placeHolder, double newValue)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | String | 单元格占位符 |
| newValue | Double | 替换双精度值 |

### 例子

```csharp

[C#]

Workbook workbook = new Workbook();
......
double newValue = 100.0;
workbook.Replace("AnOldValue", newValue);


[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
........
im NewValue As Double =  100.0
orkbook.Replace("AnOldValue", NewValue)
```

### 也可以看看

* class [Workbook](../../workbook)
* 命名空间 [Aspose.Cells](../../workbook)
* 部件 [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

将单元格的值替换为新的字符串数组。

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | String | 单元格占位符 |
| newValues | String[] | 要替换的字符串数组 |
| isVertical | Boolean | True - 垂直，False - 水平 |

### 例子

```csharp

[C#]

Workbook workbook = new Workbook();
......
string[] newValues = new string[]{"Tom", "Alice", "Jerry"};
workbook.Replace("AnOldValue", newValues, true);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
.............
im NewValues() As String =  New String() {"Tom", "Alice", "Jerry"}		
orkbook.Replace("AnOldValue", NewValues, True)
```

### 也可以看看

* class [Workbook](../../workbook)
* 命名空间 [Aspose.Cells](../../workbook)
* 部件 [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

用整数数组替换单元格的值。

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | String | 单元格占位符 |
| newValues | Int32[] | 要替换的整数数组 |
| isVertical | Boolean | True - Vertical, False - Horizontal |

### 例子

```csharp
[C#]

Workbook workbook = new Workbook();
......
int[] newValues = new int[]{1, 2, 3};
workbook.Replace("AnOldValue", newValues, true);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
..........
im NewValues() As Integer =  New Integer() {1, 2, 3}
orkbook.Replace("AnOldValue", NewValues, True)
```

### 也可以看看

* class [Workbook](../../workbook)
* 命名空间 [Aspose.Cells](../../workbook)
* 部件 [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

用双精度数组替换单元格的值。

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | String | 单元格占位符 |
| newValues | Double[] | 双数组替换 |
| isVertical | Boolean | True - 垂直，False - 水平 |

### 例子

```csharp

[C#]

Workbook workbook = new Workbook();
......
double[] newValues = new double[]{1.23, 2.56, 3.14159};
workbook.Replace("AnOldValue", newValues, true);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
...........
Dim NewValues() As Double =  New Double() {1.23, 2.56, 3.14159}
workbook.Replace("AnOldValue", NewValues, True)
```

### 也可以看看

* class [Workbook](../../workbook)
* 命名空间 [Aspose.Cells](../../workbook)
* 部件 [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

将单元格的值替换为DataTable中的数据。

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | String | 单元格占位符 |
| insertTable | DataTable | DataTable 替换 |

### 例子

```csharp
[C#]

Workbook workbook = new Workbook();
DataTable myDataTable = new DataTable("Customers");
 // 将数据添加到 myDataTable
........
workbook.Replace("AnOldValue", myDataTable);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
Dim myDataTable As DataTable =  New DataTable("Customers") 
' Adds data to myDataTable
............
workbook.Replace("AnOldValue", myDataTable)
```

### 也可以看看

* class [Workbook](../../workbook)
* 命名空间 [Aspose.Cells](../../workbook)
* 部件 [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

用新数据替换单元格的值。

```csharp
public int Replace(bool boolValue, object newValue)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| boolValue | Boolean | 要替换的布尔值。 |
| newValue | Object | 新值。可以是字符串、整数、双精度或日期时间值。 |

### 也可以看看

* class [Workbook](../../workbook)
* 命名空间 [Aspose.Cells](../../workbook)
* 部件 [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

用新数据替换单元格的值。

```csharp
public int Replace(int intValue, object newValue)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| intValue | Int32 | 要替换的整数值。 |
| newValue | Object | 新值。可以是字符串、整数、双精度或日期时间值。 |

### 也可以看看

* class [Workbook](../../workbook)
* 命名空间 [Aspose.Cells](../../workbook)
* 部件 [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

将单元格的值替换为新字符串。

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | String | 单元格占位符 |
| newValue | String | 要替换的字符串值 |
| options | ReplaceOptions | 替换选项 |

### 也可以看看

* class [ReplaceOptions](../../replaceoptions)
* class [Workbook](../../workbook)
* 命名空间 [Aspose.Cells](../../workbook)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
