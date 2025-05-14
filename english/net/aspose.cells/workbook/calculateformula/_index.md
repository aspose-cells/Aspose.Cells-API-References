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
public void Workbook_Method_CalculateFormula()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Cell cell = cells[0, 1];
    cell.Formula = "=A1>=-1";
    workbook.CalculateFormula();
    Assert.AreEqual(true, cell.BoolValue);
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
public void Workbook_Method_CalculateFormula()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    for (int i = 0; i < 5; i++)
    {
        cells[1, i].PutValue(i);
    }
    cells[3, 0].SetSharedFormula("=HLOOKUP(A1,$A$1:$E$2,2,FALSE)", 1, 5);
    wb.CalculateFormula(false);
    for (int i = 0; i < 5; i++)
    {
        Assert.AreEqual("#N/A", cells[3, i].StringValue, ((char)('A' + i)) + "4");
    }
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
// Called: wb.CalculateFormula(new CalculationOptions());
public void Workbook_Method_CalculateFormula()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    sheet.ListObjects.Add(0, 0, 1, 2, true);
    ListObject t = sheet.ListObjects[0];
    t.DisplayName = "T";
    t.ListColumns[0].Name = "A";
    t.ListColumns[1].Name = "B";
    t.ListColumns[1].Name = "C";
    Cells cells = sheet.Cells;
    cells[1, 0].PutValue("E");
    cells[1, 1].Formula = "=INDIRECT(\"T[\"&[A]&\"]\")";
    cells[1, 2].Formula = "=IFERROR(INDIRECT(\"T[\"&[A]&\"]\"),\"OK\")";
    wb.CalculateFormula(new CalculationOptions());
    Assert.AreEqual("#REF!", cells[1, 1].StringValue, "Calculating INDIRECT with invalid table reference with bracket");
    Assert.AreEqual("#REF!", cells[1, 1].StringValue, "Calculating IFERROR with invalid table reference with bracket");
}
```

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


