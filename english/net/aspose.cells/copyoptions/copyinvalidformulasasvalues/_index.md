---
title: CopyOptions.CopyInvalidFormulasAsValues
second_title: Aspose.Cells for .NET API Reference
description: CopyOptions property. If the formula is not valid for the dest destination only copy values
type: docs
url: /net/aspose.cells/copyoptions/copyinvalidformulasasvalues/
---
## CopyOptions.CopyInvalidFormulasAsValues property

If the formula is not valid for the dest destination, only copy values.

```csharp
public bool CopyInvalidFormulasAsValues { get; set; }
```

### Examples

```csharp
// Called: co.CopyInvalidFormulasAsValues = true;
public void CopyOptions_Property_CopyInvalidFormulasAsValues()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm");
    Worksheet sheet = workbook.Worksheets["300-1"];
    Workbook nb = new Workbook();
    CopyOptions co = new CopyOptions();
    co.CopyInvalidFormulasAsValues = true;
    nb.Worksheets[0].Copy(sheet, co);
    Assert.AreEqual("日本",nb.Worksheets[0].Validations[2].Formula1);
    Util.ReSave(nb, SaveFormat.Xlsx);
    //nb.Save(Constants.destPath + "dest.xlsx");
}
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


