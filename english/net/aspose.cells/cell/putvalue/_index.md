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
// Called: cells[2, 0].PutValue(true);
[Test, Ignore("Not ready to test this yet")]
        public void Method_Boolean_()
        {
            caseName = "testRangeCopy_Excel2007_001";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue(1);
            cells[1, 0].PutValue("abc");
            cells[2, 0].PutValue(true);
            cells[3, 0].PutValue(2.16);
            Aspose.Cells.Range rangeSrc = cells.CreateRange(0, 0, 4, 1);
            Aspose.Cells.Range rangeDest = cells.CreateRange(1048572, 16383, 4, 1); 
            rangeDest.Copy(rangeSrc);

            checkRangeCopy_Excel2007_001(workbook);
            workbook.Save(Constants.destPath + "testRangeCopy.xlsx");
            workbook = new Workbook(Constants.destPath + "testRangeCopy.xlsx");
            checkRangeCopy_Excel2007_001(workbook);
            workbook.Save(Constants.destPath + "testRangeCopy.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testRangeCopy.xml");
            checkRangeCopy_Excel2007_001(workbook);
            workbook.Save(Constants.destPath + "testRangeCopy.xls");
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
// Called: cells[1, 2].PutValue(9);
[Test]
      public void Method_Int32_()
      {
        Workbook workbook = new Workbook();
        Cells cells = workbook.Worksheets[0].Cells;
        cells[0, 0].PutValue("Axles");
        cells[1, 0].PutValue(4);
        cells[2, 0].PutValue(5);
        cells[3, 0].PutValue(6);
        cells[0, 1].PutValue("Bearings");
        cells[1, 1].PutValue(4);
        cells[2, 1].PutValue(7);
        cells[3, 1].PutValue(8);
        cells[0, 2].PutValue("Bolts");
        cells[1, 2].PutValue(9);
        cells[2, 2].PutValue(10);
        cells[3, 2].PutValue(11);
        Cell cell = cells[0, 3];
        cell.Formula = "=HLOOKUP(3,A2:C4,2,false)";
        workbook.CalculateFormula();
        Assert.AreEqual("#N/A", cell.StringValue);
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
// Called: cells[3, 1].PutValue(0.55);
[Test]
        public void Method_Double_()
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
            cell.Formula = "=INDEX(A2:C5,2.8,3)";
            workbook.CalculateFormula();
            Assert.AreEqual(38, cell.IntValue);
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
// Called: cells["A1"].PutValue("12:40", true, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("12:40", true, true);
            Assert.AreEqual(cells["A1"].GetStyle().IsDateTime, true);
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
// Called: cells[2, 4].PutValue("TOO", true);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[2, 2].PutValue("COUNT", true);
            cells[2, 3].PutValue("ME", true);
            cells[2, 4].PutValue("TOO", true);
            cells[3, 1].Formula = "=COUNTA(INDIRECT(\"A3:IV3\"))";
            wb.CalculateFormula();
            Assert.AreEqual("3", cells[3, 1].StringValue);
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
// Called: cells[2, 0].PutValue("Orange");
[Test]
    public void Method_String_()
    {
      Workbook workbook = new Workbook();
      Cells cells = workbook.Worksheets[0].Cells;
      cells[0, 0].PutValue("Apple");
      cells[1, 0].PutValue("Banana");
      cells[2, 0].PutValue("Orange");
      cells[0, 1].PutValue(1);
      cells[1, 1].PutValue(2);
      cells[2, 1].PutValue(3);
      cells[0, 2].Formula = "=SUMIF(A1:A3,\"red\",B1:B3)";
      workbook.CalculateFormula();
      Console.WriteLine("=SUMIF(A1:A3,\"red\",B1:B3)");
      Assert.AreEqual(0, cells[0, 2].IntValue);
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
// Called: cells[1, 0].PutValue(dt);
[Test]
      public void Method_Object_()
      {
        Workbook workbook = new Workbook();
        Cells cells = workbook.Worksheets[0].Cells;
        cells[0, 0].PutValue("aspose");
        DateTime dt = new DateTime(2008, 12, 8);
        cells[1, 0].PutValue(dt);
        cells[3, 0].PutValue(19);
        cells[4, 0].PutValue(22.6);
        cells[5, 0].PutValue(true);
        cells[6, 0].PutValue("");
        cells[7, 0].PutValue("#DIV/0!");
        cells[0, 1].Formula = "=COUNTA(A1:A8)";
        workbook.CalculateFormula();
        Assert.AreEqual(7, cells[0, 1].IntValue);
      }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


