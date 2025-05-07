---
title: Workbook.GetNamedStyle
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Gets the named style in the style pool
type: docs
url: /net/aspose.cells/workbook/getnamedstyle/
---
## Workbook.GetNamedStyle method

Gets the named style in the style pool.

```csharp
public Style GetNamedStyle(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | name of the style |

### Return Value

named style, maybe null.

### Examples

```csharp
// Called: Style style = workbook.GetNamedStyle("SecondaryStyle_Locked");
public void Method_String_()
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
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


