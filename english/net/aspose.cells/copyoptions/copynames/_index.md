---
title: CopyOptions.CopyNames
second_title: Aspose.Cells for .NET API Reference
description: CopyOptions property. Indicates whether copying the names
type: docs
url: /net/aspose.cells/copyoptions/copynames/
---
## CopyOptions.CopyNames property

Indicates whether copying the names.

```csharp
public bool CopyNames { get; set; }
```

### Examples

```csharp
// Called: CopyNames = true
public static void Property_CopyNames()
        {
            var outputWb = new Workbook();
            var wb = new Workbook(Constants.destPath + &quot;CellsNet45795.xlsx&quot;);

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
            OutputValidations(outputWb, &quot;CopyBook&quot;);
            Util.ReSave(outputWb, SaveFormat.Xlsx);
            //outputWb.Save(Constants.destPath + &quot;CopyCellsNet45795.xlsx&quot;);
        }
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


