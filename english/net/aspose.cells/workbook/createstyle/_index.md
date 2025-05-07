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
// Called: style = worksheet.Workbook.CreateStyle();
[Test]
        public void Method_CreateStyle()
        {
            var workbook = new Workbook();
            workbook.Settings.UpdateAdjacentCellsBorder = true;
            var worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].Value = "hello";
            //create range and style and apply horizontal style to A1 cell
            var range = worksheet.Cells.CreateRange(0, 0, 1, 1);
            var style = worksheet.Workbook.CreateStyle();
            var flag = new StyleFlag();
            style.HorizontalAlignment = TextAlignmentType.Center;
            flag.HorizontalAlignment = true;
            range.ApplyStyle(style, flag);

            //create another range and style and apply vertical alignment to A1 cell
            range = worksheet.Cells.CreateRange(0, 0, 1, 1);
            style = worksheet.Workbook.CreateStyle();
            flag = new StyleFlag();
            style.VerticalAlignment = TextAlignmentType.Center;
            flag.VerticalAlignment = true;
            range.ApplyStyle(style, flag);

            workbook.Save(Constants.destPath + "CellsNet45814.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet45814.xlsx");
            Assert.AreEqual(TextAlignmentType.Center, workbook.Worksheets[0].Cells["A1"].GetStyle().VerticalAlignment);
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
            cells[0, 0].PutValue("In original template file, there are two data sheets and one eval sheet");
            cells[1, 0].PutValue("The first eval sheet comes from template so it does not indicate license status");
            Style style = wb.CreateStyle(false);
            style.Font.Color = System.Drawing.Color.Pink;
            Cell cell = cells[3, 0];
            cell.SetStyle(style);
            cell.PutValue(hintValue);
            cell = cells[5, 0];
            style.Font.Size = 13;
            cell.SetStyle(style);
            cell.SetFormula("=\"Value AFTER calculation\"", "Value BEFORE calculation");
            cells = wb.Worksheets.Add("Sheet2").Cells;
            cells[0, 0].PutValue("This is data in the second sheet");
            return wb;
        }
```

### See Also

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


