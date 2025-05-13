---
title: CopyOptions.ReferToSheetWithSameName
second_title: Aspose.Cells for .NET API Reference
description: CopyOptions property. In ms excel when copying formulas which refer to other worksheets while copying a worksheet to another one the copied formulas should refer to source workbook. However for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook such as when those worksheets have been copied before this copy operation then this property should be kept as true
type: docs
url: /net/aspose.cells/copyoptions/refertosheetwithsamename/
---
## CopyOptions.ReferToSheetWithSameName property

In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true.

```csharp
public bool ReferToSheetWithSameName { get; set; }
```

### Remarks

The default value is true.

### Examples

```csharp
// Called: options.ReferToSheetWithSameName = true;
public void CopyOptions_Property_ReferToSheetWithSameName()
{
    string templetePath = Constants.sourcePath + "example.xlsx";
    Workbook templeteWorkbook = new Aspose.Cells.Workbook(templetePath);
    Workbook outputWorkbook = new Aspose.Cells.Workbook();

    for (int i = 0; i < templeteWorkbook.Worksheets.Count; i++)
    {
        outputWorkbook.Worksheets.Add(templeteWorkbook.Worksheets[i].Name);
    }
    for (int i = 0; i < templeteWorkbook.Worksheets.Count; i++)
    {
        Aspose.Cells.CopyOptions options = new Aspose.Cells.CopyOptions();
        options.ReferToSheetWithSameName = true;
        outputWorkbook.Worksheets[templeteWorkbook.Worksheets[i].Name].Copy(templeteWorkbook.Worksheets[i]);
    }

    outputWorkbook.Worksheets.RemoveAt(0);
    outputWorkbook.Worksheets.RemoveAt("Start");
    outputWorkbook.Worksheets.RemoveAt("End");
    Assert.AreEqual("=SUM(Detail!B3)", outputWorkbook.Worksheets[0].Cells["B3"].Formula);
}
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


