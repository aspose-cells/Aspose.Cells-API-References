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
// Called: if (ws.Type == SheetType.Chart)
[Test]
        public void Type_SheetType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Test162141.xls");
            foreach (Worksheet ws in workbook.Worksheets)
            {
                if (ws.Type == SheetType.Chart)
                    continue;

                int index = 0;
                foreach (Picture picture in ws.Pictures)
                {
                    //save the image:
                    byte[] data = picture.Data;
                    if (data != null)
                    {
#if !NETCOREAPP2_0
                        Bitmap bmp = new Bitmap(new MemoryStream(data));
                        bmp.Save(Constants.destPath + (index++) + ".bmp", ImageFormat.Bmp);
#endif
                    }                  
                }
            }

            workbook.Save(Constants.destPath + "Test162141.xls");
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


