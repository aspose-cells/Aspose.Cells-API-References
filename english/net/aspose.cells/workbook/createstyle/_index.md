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
// Called: Style newStyle = checkExcel.CreateStyle();
private bool Workbook_Method_CreateStyle(string filePath, Workbook checkExcel, HtmlSaveOptions saveOptions)
        {
            bool result = true;
            int sheetCount = checkExcel.Worksheets.Count;
            Worksheet worksheet = null;
            try
            {
                for (int i = 1; i <= sheetCount; i++)
                {
                    worksheet = checkExcel.Worksheets[i - 1];
                    if (worksheet != null && worksheet.IsVisible)
                    {
                        Style newStyle = checkExcel.CreateStyle();
                        newStyle.IsTextWrapped = true;
                        StyleFlag flag = new StyleFlag();
                        flag.WrapText = true;
                        newStyle.IsTextWrapped = true;
                        Cells cells = worksheet.Cells;
                        cells.ApplyStyle(newStyle, flag);
                        checkExcel.Worksheets.ActiveSheetIndex = i - 1;
                        checkExcel.Save(CreateFolder(filePath) + "canapplystle.html", saveOptions);
                    }
                }
            }
            catch (Exception e)
            {
                result = false;
            }
            return result;
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
private Workbook Workbook_Method_CreateStyle(string hintValue)
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


