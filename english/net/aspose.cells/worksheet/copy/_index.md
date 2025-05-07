---
title: Worksheet.Copy
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Copies contents and formats from another worksheet
type: docs
url: /net/aspose.cells/worksheet/copy/
---
## Copy(Worksheet) {#copy}

Copies contents and formats from another worksheet.

```csharp
public void Copy(Worksheet sourceSheet)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | Worksheet | Source worksheet. |

### Examples

```csharp
// Called: destinationWorksheet2.Copy(sourceWorksheet);
[Test]
        public void Method_Worksheet_()
        {
            Workbook sourceWorkbook = new Workbook(Constants.sourcePath + "Copy Formats Issue.xlsb");
            Worksheet sourceWorksheet = sourceWorkbook.Worksheets[0];
            Workbook destinationWorkbook = new Workbook();
            Worksheet destinationWorksheet1 = destinationWorkbook.Worksheets.Insert(0, SheetType.Worksheet);
            destinationWorksheet1.Copy(sourceWorksheet);
            Worksheet destinationWorksheet2 = destinationWorkbook.Worksheets.Insert(0, SheetType.Worksheet);
            destinationWorksheet2.Copy(sourceWorksheet);
            Assert.AreEqual(destinationWorksheet2.Cells["A1"].GetStyle().IsTextWrapped, true);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Worksheet, CopyOptions) {#copy_1}

Copies contents and formats from another worksheet.

```csharp
public void Copy(Worksheet sourceSheet, CopyOptions copyOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | Worksheet | Source worksheet. |
| copyOptions | CopyOptions |  |

### Remarks

You can copy data from another worksheet in the same file or another file. However, this method does not support to copy drawing objects, such as comments, images and charts.

### Examples

```csharp
// Called: outputWs.Copy(ws, new CopyOptions()
public static void Method_CopyOptions_()
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

* class [CopyOptions](../../copyoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


