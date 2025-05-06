---
title: Workbook.CreateStyle
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Creates a new style
type: docs
url: /net/aspose.cells/workbook/createstyle/
---
## CreateStyle() {#createstyle}

Creates a new style.

```csharp
public Style CreateStyle()
```

### Return Value

Returns a style object.

### Examples

```csharp
// Called: Style style = workbook.CreateStyle();
[Test]
    public void Method_CreateStyle()
    {
      Workbook workbook = new Workbook();
#if NETCOREAPP2_0
      workbook.Settings.CultureInfo = new System.Globalization.CultureInfo(&quot;en-US&quot;);
#endif
      Cells cells = workbook.Worksheets[0].Cells;
      Style style = workbook.CreateStyle();
      style.Custom = &quot;$#,##0_);($#,##0)&quot;;
      cells[0, 0].PutValue(10);
      cells[0, 0].SetStyle(style);
      cells[0, 1].Formula = &quot;=CELL(\&quot;format\&quot;, A1)&quot;;
      Console.WriteLine(&quot;=CELL(\&quot;format\&quot;, A1)&quot;);
      workbook.CalculateFormula();
      Assert.AreEqual(&quot;C0&quot;, cells[0, 1].StringValue);
    }
```

### See Also

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateStyle(bool) {#createstyle_1}

Creates a new style.

```csharp
public Style CreateStyle(bool cloneDefaultStyle)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cloneDefaultStyle | Boolean | Incidates whether clones the default style |

### Return Value

Returns a style object.

### Examples

```csharp
// Called: Style style = wb.CreateStyle(false);
private Workbook Method_Boolean_(string hintValue)
        {
            Workbook wb = new Workbook();
            wb.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            Worksheet sheet = wb.Worksheets[0];
            sheet.PageSetup.PrintGridlines = true;
            Cells cells = sheet.Cells;
            cells[0, 0].PutValue(&quot;In original template file, there are two data sheets and one eval sheet&quot;);
            cells[1, 0].PutValue(&quot;The first eval sheet comes from template so it does not indicate license status&quot;);
            Style style = wb.CreateStyle(false);
            style.Font.Color = System.Drawing.Color.Pink;
            Cell cell = cells[3, 0];
            cell.SetStyle(style);
            cell.PutValue(hintValue);
            cell = cells[5, 0];
            style.Font.Size = 13;
            cell.SetStyle(style);
            cell.SetFormula(&quot;=\&quot;Value AFTER calculation\&quot;&quot;, &quot;Value BEFORE calculation&quot;);
            cells = wb.Worksheets.Add(&quot;Sheet2&quot;).Cells;
            cells[0, 0].PutValue(&quot;This is data in the second sheet&quot;);
            return wb;
        }
```

### See Also

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


