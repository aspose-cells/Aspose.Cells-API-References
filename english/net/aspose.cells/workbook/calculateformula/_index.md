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
[Test, Ignore("Not ready to test this yet")]
        public void Method_CalculateFormula()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue(1);
            cells[1, 0].PutValue(9);
            cells[2, 0].PutValue(5);
            cells[3, 0].PutValue(7);
            cells[0, 1].PutValue(0);
            cells[1, 1].PutValue(4);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[5, 0].SetArrayFormula("=LINEST(A1:A4,B1:B4,FALSE,FALSE)", 1, 2);
            workbook.CalculateFormula();
            Assert.AreEqual(2.3103, cells[5, 0].DoubleValue, 0.0001);
            Assert.AreEqual(0, cells[5, 1].DoubleValue, 0.0001);
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
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i < 6; i++)
            {
                cells[i / 2, i % 2].PutValue(0x01 << i);
            }
            Cell cell = cells[0, 2];
            cell.Formula = "=SUMPRODUCT(A3:OFFSET(A3,-2,0),1-B3:OFFSET(B3,-2,0))";
            wb.CalculateFormula(false);
            Assert.AreEqual(-525.0, cell.DoubleValue, "Range operator in array");
            cell.Formula = "=SUMPRODUCT(A3:OFFSET(A3,-2,0),-B3:OFFSET(B3,-2,0))";
            wb.CalculateFormula(false);
            Assert.AreEqual(-546.0, cell.DoubleValue, "Range operator in array");
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
// Called: wb.CalculateFormula(copts);
[Test]
        public void Method_CalculationOptions_()
        {
            Workbook wb = new Workbook();
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.Formula = "=HYPERLINK(\"http://localhost:9090\",\"Target\")";
            CustomEngineForHyperlink cffh = new CustomEngineForHyperlink(true);
            CalculationOptions copts = new CalculationOptions();
            copts.CustomEngine = cffh;
            wb.CalculateFormula(copts);
            if (!cffh.Invoked)
            {
                Assert.Fail("HYPERLINK in custom engine should be called");
            }
            cffh = new CustomEngineForHyperlink(false);
            copts = new CalculationOptions();
            copts.CustomEngine = cffh;
            wb.CalculateFormula(copts);
            if (cffh.Invoked)
            {
                Assert.Fail("HYPERLINK in custom engine should not be called");
            }
        }
```

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


