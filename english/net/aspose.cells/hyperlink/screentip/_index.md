---
title: Hyperlink.ScreenTip
second_title: Aspose.Cells for .NET API Reference
description: Hyperlink property. Returns or sets the ScreenTip text for the specified hyperlink
type: docs
url: /net/aspose.cells/hyperlink/screentip/
---
## Hyperlink.ScreenTip property

Returns or sets the ScreenTip text for the specified hyperlink.

```csharp
public string ScreenTip { get; set; }
```

### Examples

```csharp
// Called: worksheet.Hyperlinks[hLinkIdx].ScreenTip = "Go to workbook containing this formula.";
private static void Hyperlink_Property_ScreenTip(Worksheet worksheet, int rowIdx, string workbookPath, string sheetName, string cellAddress)
        {
            string hyperlinkString = workbookPath+"#'"+sheetName.Replace("'", "''")+"'!"+cellAddress;

            int hLinkIdx = worksheet.Hyperlinks.Add(rowIdx + 1, 0, 1, 5, hyperlinkString);

            worksheet.Hyperlinks[hLinkIdx].ScreenTip = "Go to workbook containing this formula.";

        }
```

### See Also

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


