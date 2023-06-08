---
title: Cell.PutValue
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Puts a boolean value into the cell
type: docs
url: /net/aspose.cells/cell/putvalue/
---
## PutValue(bool) {#putvalue}

Puts a boolean value into the cell.

```csharp
public void PutValue(bool boolValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| boolValue | Boolean |  |

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(int) {#putvalue_2}

Puts an integer value into the cell.

```csharp
public void PutValue(int intValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| intValue | Int32 | Input value |

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(double) {#putvalue_1}

Puts a double value into the cell.

```csharp
public void PutValue(double doubleValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| doubleValue | Double | Input value |

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool, bool) {#putvalue_7}

Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
| isConverted | Boolean | True: converted to other data type if appropriate. |
| setStyle | Boolean | True: set the number format to cell's style when converting to other data type |

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool) {#putvalue_6}

Puts a string value into the cell and converts the value to other data type if appropriate.

```csharp
public void PutValue(string stringValue, bool isConverted)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
| isConverted | Boolean | True: converted to other data type if appropriate. |

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string) {#putvalue_5}

Puts a string value into the cell.

```csharp
public void PutValue(string stringValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(DateTime) {#putvalue_3}

Puts a DateTime value into the cell.

```csharp
public void PutValue(DateTime dateTime)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dateTime | DateTime | Input value |

### Remarks

Setting a DateTime value for a cell dose not means the cell will be formatted as date time automatically. DateTime value was maintained as numeric value in the data model of both ms excel and Aspose.Cells. Whether the numeric value will be taken as the numeric value itself or date time depends on the number format applied on this cell. If this cell has not been formatted as date time, it will be displayed as a numeric value even though what you input is DateTime.

### Examples

This example shows how to set DateTime value to a cell and make it be displayed as date time.

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Put date time into a cell
Cell cell = cells[0, 0];
cell.PutValue(new DateTime(2023, 5, 15));
Style style = cell.GetStyle(false);
style.Number = 14;
cell.SetStyle(style);
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(object) {#putvalue_4}

Puts an object value into the cell.

```csharp
public void PutValue(object objectValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| objectValue | Object | input value |

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


