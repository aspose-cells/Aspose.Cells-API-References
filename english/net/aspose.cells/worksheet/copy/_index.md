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
// Called: _workSheetDeco.Copy(_template_DecoSheet); //Exception here
public void Worksheet_Method_Copy()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet _template_DecoSheet = workbook.Worksheets[0];

    Workbook _parentBook = new Workbook();
    Worksheet _workSheetDeco = _parentBook.Worksheets[0];
    _workSheetDeco.Copy(_template_DecoSheet); //Exception here 
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
// Called: wtemp.Worksheets[1].Copy(old.Worksheets[1], options);
public void Worksheet_Method_Copy()
{
    var excelPath = Constants.sourcePath + "example.xlsx";
    var excelpath1 = Constants.sourcePath + "example.xlsx";

    Workbook old = new Workbook(excelPath);
    Workbook wtemp = new Workbook(excelpath1);
    CopyOptions options = new CopyOptions();
    //  options.ReferToSheetWithSameName = true;
    wtemp.Worksheets[1].Copy(old.Worksheets[1], options);
    Assert.AreEqual("=Sheet1!c_4", wtemp.Worksheets[1].Cells["A1"].Formula);
    Util.ReSave(wtemp, SaveFormat.Xlsx);
    //wtemp.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [CopyOptions](../../copyoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


