---
title: Cell.SetStyle
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Sets the cell style
type: docs
url: /net/aspose.cells/cell/setstyle/
---
## SetStyle(Style) {#setstyle}

Sets the cell style.

```csharp
public void SetStyle(Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |

### Remarks

If the border settings are changed, the border of adjust cells will be updated too.

### Examples

```csharp
// Called: cells[1, 1].SetStyle(style);
public void Cell_Method_SetStyle()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Style style = cells[1, 1].GetStyle();
    style.Pattern = BackgroundType.Solid;
    cells[1, 1].SetStyle(style);

    checkBackgroundType_Solid(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    checkBackgroundType_Solid(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    checkBackgroundType_Solid(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
    checkBackgroundType_Solid(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003); 
}
```

### See Also

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, bool) {#setstyle_2}

Apply the changed property of style to the cell.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| explicitFlag | Boolean | True, only overwriting formatting which is explicitly set. |

### Examples

```csharp
// Called: cell.SetStyle(style, true);
public void Cell_Method_SetStyle()
        {
            Workbook workbook = new Workbook(USBankConstants.sourcePath + "Styles.xlsx");

            Style style = workbook.GetNamedStyle("SecondaryStyle_Locked");
            Cell cell = workbook.Worksheets[0].Cells["B2"];
            cell.SetStyle(style, true);

            style = workbook.GetNamedStyle("SecondaryStyle_LockedHidden");
            cell = workbook.Worksheets[0].Cells["B3"];
            cell.SetStyle(style, true);

            string output = USBankConstants.resultPath + "Styles_result.xlsx";
            workbook.Save(output);
           
        }
```

### See Also

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, StyleFlag) {#setstyle_1}

Apply the cell style based on flags.

```csharp
public void SetStyle(Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| flag | StyleFlag | The style flag. |

### Examples

```csharp
// Called: mycell.SetStyle(style, flag);
public void Cell_Method_SetStyle()
{
    Workbook workbook = new Workbook();
    Worksheet sheet = workbook.Worksheets[0];
    Style style = workbook.CreateStyle();
    style.Font.Color = (Color.Red);
    style.Name = ("Style1");
    StyleFlag flag = new StyleFlag();
    flag.All = (true);
    Cells mycells = sheet.Cells;
    Cell mycell = mycells["A1"];
    mycell.PutValue("Tekst");
    mycell.SetStyle(style, flag);
    //Saving the Excel file 
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    style = workbook.Worksheets[0].Cells["A1"].GetStyle();
    Assert.AreEqual(style.ParentStyle.Name, "Style1");
}
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


