---
title: StyleFlag.WrapText
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Wrap text setting will be applied
type: docs
url: /net/aspose.cells/styleflag/wraptext/
---
## StyleFlag.WrapText property

Wrap text setting will be applied.

```csharp
public bool WrapText { get; set; }
```

### Examples

```csharp
// Called: flag.WrapText = true;
private bool StyleFlag_Property_WrapText(string filePath, Workbook checkExcel, HtmlSaveOptions saveOptions)
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

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


