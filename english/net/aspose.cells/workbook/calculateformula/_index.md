---
title: Workbook.CalculateFormula
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Calculates the result of formulas
type: docs
url: /net/aspose.cells/workbook/calculateformula/
---
## CalculateFormula() {#calculateformula}

Calculates the result of formulas.

```csharp
public void CalculateFormula()
```

### Remarks

For all supported formulas, please see the list at https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### Examples

```csharp
// Called: workbook.CalculateFormula();
[Test, ExpectedException(typeof(CellsException))] 
#endif
    public void Method_CalculateFormula()
    {
      Workbook workbook = new Workbook();
      Cells cells = workbook.Worksheets[0].Cells;
      cells[0, 0].Formula = &quot;=PRODUCT()&quot;;
      workbook.CalculateFormula();
    }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(bool) {#calculateformula_2}

Calculates the result of formulas.

```csharp
public void CalculateFormula(bool ignoreError)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ignoreError | Boolean | Indicates if hide the error in calculating formulas. The error may be unsupported function, external links, etc. |

### Examples

```csharp
// Called: wb.CalculateFormula(false);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.France;
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell1 = cells[0, 0];
            Cell cell2 = cells[0, 1];
            Cell cell3 = cells[0, 2];
            string es = wb.Settings.CultureInfo.NumberFormat.NumberGroupSeparator;
            cell1.Formula = &quot;=TEXT(123456789,\&quot;#&quot; + es + &quot;###\&quot;)&quot;;
            cell2.Formula = &quot;=TEXT(123456789,\&quot;# ###\&quot;)&quot;;
            cell3.Formula = &quot;=TEXT(123456789,\&quot;# ##\&quot;)&quot;;
            wb.CalculateFormula(false);
            es = &quot;123&quot; + es + &quot;456&quot; + es + &quot;789&quot;;
            Assert.AreEqual(es, cell1.StringValue, cell1.Formula);
            Assert.AreEqual(es, cell2.StringValue, cell2.Formula);
            Assert.AreEqual(es, cell3.StringValue, cell3.Formula);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(CalculationOptions) {#calculateformula_1}

Calculating formulas in this workbook.

```csharp
public void CalculateFormula(CalculationOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options for calculation |

### Examples

```csharp
// Called: wb.CalculateFormula(new CalculationOptions() { CustomEngine = new CustomFunction() });
[Test]
        public void Method_CalculationOptions_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Create table with data
            var range = cells.CreateRange(&quot;B3:D5&quot;);
            range.Value = new object[,]
            {
            {&quot;AccountNum&quot;, &quot;UDF&quot;, &quot;Normal&quot;},
            {&quot;Row01&quot;, &quot;&quot;, &quot;&quot;},
            {&quot;Row02&quot;, &quot;&quot;, &quot;&quot;},
            };
            int firstRow = range.FirstRow;
            int firstColumn = range.FirstColumn;
            int endRow = firstRow + range.RowCount;
            int endColumn = firstColumn + range.ColumnCount;
            sheet.ListObjects.Add(firstRow, firstColumn, endRow, endColumn, true);

            // Populate formulas
            cells[&quot;C5&quot;].Formula =
            cells[&quot;C4&quot;].Formula = &quot;=UDFTest([@AccountNum])&quot;; // UDF formula

            cells[&quot;D5&quot;].Formula =
            cells[&quot;D4&quot;].Formula = &quot;=[@AccountNum]&quot;; // Built-in formula comparison

            // Calculate workbook
            wb.CalculateFormula(new CalculationOptions() { CustomEngine = new CustomFunction() });

            Assert.AreEqual(&quot;Row01&quot;, cells[&quot;C4&quot;].Value, &quot;C4&quot;);
            Assert.AreEqual(&quot;Row02&quot;, cells[&quot;C5&quot;].Value, &quot;C5&quot;);
            Assert.AreEqual(&quot;Row01&quot;, cells[&quot;D4&quot;].Value, &quot;D4&quot;);
            Assert.AreEqual(&quot;Row02&quot;, cells[&quot;D5&quot;].Value, &quot;D5&quot;);
        }
```

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


