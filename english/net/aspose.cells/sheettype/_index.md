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
// Called: Assert.AreEqual(workbook.Worksheets[0].Type, SheetType.InternationalMacro);
[Test]
        public void Type_SheetType()
        {  // workbook.Save(dir + &quot;dest.xlsx&quot;);
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-47410.xlsm&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Type, SheetType.InternationalMacro);
            workbook.Save(Constants.destPath + &quot;CELLSNET-47410.xlsm&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET-47410.xlsm&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Type, SheetType.InternationalMacro);
            workbook.Save(Constants.destPath + &quot;CELLSNET-47410.xlsb&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET-47410.xlsb&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Type, SheetType.InternationalMacro);
            workbook.Save(Constants.destPath + &quot;CELLSNET-47410.xlsm&quot;);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


