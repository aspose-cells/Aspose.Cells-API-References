---
title: Enum SheetType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.SheetType enum. Specifies the worksheet type
type: docs
url: /net/aspose.cells/sheettype/
---
## SheetType enumeration

Specifies the worksheet type.

```csharp
public enum SheetType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| VB | `0` | Visual Basic module |
| Worksheet | `1` |  |
| Chart | `2` | Chart |
| BIFF4Macro | `3` | BIFF4 Macro sheet |
| InternationalMacro | `4` | International Macro sheet |
| Other | `5` |  |
| Dialog | `6` | Dialog worksheet |

### Examples

```csharp
// Called: loOrigWB.Worksheets.Insert(0, SheetType.Worksheet).Copy(loOrigWS);
public void Cells_Type_SheetType()
{
    string filePath = Constants.PivotTableSourcePath + @"NET46587_";

    Workbook loOrigWB = new Workbook(filePath + @"Orig.xlsx");
    Worksheet loOrigWS = loOrigWB.Worksheets["Sheet1"];
    loOrigWB.Worksheets.Insert(0, SheetType.Worksheet).Copy(loOrigWS);
    var loNewWS = loOrigWB.Worksheets["Sheet2"];
    loNewWS.Cells.DeleteRows(0, 3);
    loNewWS.Cells.DeleteColumns(0, 3, true);
    loNewWS.RefreshPivotTables();
    loNewWS.Charts[0].RefreshPivotData();
    loOrigWB.Save(Constants.PIVOT_CHECK_FILE_PATH + @"example.xlsx");
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


