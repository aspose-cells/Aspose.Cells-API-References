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

### Examples

```csharp
// Called: cells[2, 2].PutValue(true);
public void Cell_Method_PutValue()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells[1, 1].PutValue("FfalseL");
    cells[2, 2].PutValue(true);

    CheckFind_EndWith_006(workbook);
}
```

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

### Examples

```csharp
// Called: cells[4, 0].PutValue(8);
public void Cell_Method_PutValue()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells[0, 0].PutValue(3);
    cells[1, 0].PutValue(3);
    cells[2, 0].PutValue(4);
    cells[3, 0].PutValue(6);
    cells[4, 0].PutValue(8);
    Cell cell = cells[0, 1];
    cell.Formula = "=MATCH(3,A1:A5,1)";
    workbook.CalculateFormula();
    Assert.AreEqual(2, cell.IntValue);
}
```

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

### Examples

```csharp
// Called: cells[2, 1].PutValue(0.69);
public void Cell_Method_PutValue()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells[0, 0].PutValue("Fruit");
    cells[0, 1].PutValue("Price");
    cells[0, 2].PutValue("Count");
    cells[1, 0].PutValue("Apples");
    cells[1, 1].PutValue(0.69);
    cells[1, 2].PutValue(40);
    cells[2, 0].PutValue("Bananas");
    cells[2, 1].PutValue(0.69);
    cells[2, 2].PutValue(38);
    cells[3, 0].PutValue("Lemons");
    cells[3, 1].PutValue(0.55);
    cells[3, 2].PutValue(15);
    cells[4, 0].PutValue("Oranges");
    cells[4, 1].PutValue(0.25);
    cells[4, 2].PutValue(25);
    Cell cell = cells[0, 3];
    cell.Formula = "=INDEX(A2:C5,5,3)";
    workbook.CalculateFormula();
    Assert.AreEqual("#REF!", cell.StringValue);
}
```

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

### Examples

```csharp
// Called: age.PutValue("-60", true, false);
public void Cell_Method_PutValue()
 {
     var book = new Workbook(Constants.sourcePath + "example.xlsx");
     book.CalculateFormula();

     Worksheet sheetBla = book.Worksheets["Sheet1"];

     Cell age = sheetBla.Cells["B3"];
     age.PutValue("-60", true, false);
     book.CalculateFormula();
     bool isValid = age.GetValidationValue(); //
     Assert.IsFalse(isValid);
     book.Save(Constants.destPath + "example.xlsx");
           
 }
```

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

### Examples

```csharp
// Called: cells[2, 2].PutValue("1", true);
public void Cell_Method_PutValue()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells[2, 2].PutValue("1", true);
    cells[2, 3].PutValue("2", true);
    cells[2, 4].PutValue("3", true);
    //SHEET.Cells[3, 1].Formula = "=PERCENTRANK(INDIRECT(\"A3:IV3\"),INDIRECT(\"C2\"))";
    cells[3, 1].Formula = "=PERCENTRANK(A2:Z2,C2)";
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

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

### Examples

```csharp
// Called: cells[0, 1].PutValue("Price");
public void Cell_Method_PutValue()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells[0, 0].PutValue("Fruit");
    cells[0, 1].PutValue("Price");
    cells[0, 2].PutValue("Count");
    cells[1, 0].PutValue("Apples");
    cells[1, 1].PutValue(0.69);
    cells[1, 2].PutValue(40);
    cells[2, 0].PutValue("Bananas");
    cells[2, 1].PutValue(0.69);
    cells[2, 2].PutValue(38);
    cells[3, 0].PutValue("Lemons");
    cells[3, 1].PutValue(0.55);
    cells[3, 2].PutValue(15);
    cells[4, 0].PutValue("Oranges");
    cells[4, 1].PutValue(0.25);
    cells[4, 2].PutValue(25);
    Cell cell = cells[0, 3];
    cell.Formula = "=INDEX(A2:C5,2,4)";
    workbook.CalculateFormula();
    Assert.AreEqual("#REF!", cell.StringValue);
}
```

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

### Examples

```csharp
// Called: cells[0, 0].PutValue(dt);
public void Cell_Method_PutValue()
{
  Workbook workbook = new Workbook();
  Cells cells = workbook.Worksheets[0].Cells;
  DateTime dt = new DateTime(2008, 2, 2);
  cells[0, 0].PutValue(dt);
  cells[0, 1].Formula = "=EOMONTH(A1, 1)";
  workbook.CalculateFormula();
  Assert.AreEqual(39538, cells[0, 1].IntValue);
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


