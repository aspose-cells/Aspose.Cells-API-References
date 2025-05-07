---
title: Cells.ApplyStyle
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Applies formats for a whole worksheet
type: docs
url: /net/aspose.cells/cells/applystyle/
---
## Cells.ApplyStyle method

Applies formats for a whole worksheet.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### Examples

```csharp
// Called: cells.ApplyStyle(newStyle, flag);
private bool Method_StyleFlag_(string filePath, Workbook checkExcel, HtmlSaveOptions saveOptions)
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
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


