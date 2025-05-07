---
title: CopyOptions.ColumnCharacterWidth
second_title: Aspose.Cells for .NET API Reference
description: CopyOptions property. Indicates whether copying column width in unit of characters
type: docs
url: /net/aspose.cells/copyoptions/columncharacterwidth/
---
## CopyOptions.ColumnCharacterWidth property

Indicates whether copying column width in unit of characters.

```csharp
public bool ColumnCharacterWidth { get; set; }
```

### Examples

```csharp
// Called: ColumnCharacterWidth = true,
public static void Property_ColumnCharacterWidth()
        {
            var outputWb = new Workbook();
            var wb = new Workbook(Constants.destPath + "CellsNet45795.xlsx");

            foreach (Worksheet ws in wb.Worksheets)
            {

                var outputWs = outputWb.Worksheets.Add(ws.Name);
                outputWs.Copy(ws, new CopyOptions()
                {
                    ColumnCharacterWidth = true,
                    CopyInvalidFormulasAsValues = true,
                    CopyNames = true
                });
            }
            OutputValidations(outputWb, "CopyBook");
            Util.ReSave(outputWb, SaveFormat.Xlsx);
            //outputWb.Save(Constants.destPath + "CopyCellsNet45795.xlsx");
        }
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


