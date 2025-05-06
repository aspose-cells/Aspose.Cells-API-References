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
// Called: copyOptions.ReferToSheetWithSameName = true;
[Test]
        public void Property_ReferToSheetWithSameName()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet54216.xlsx&quot;);
            Workbook n = new Workbook();
            //int i = 0;
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Worksheet s = n.Worksheets.Add(sheet.Name);
                //s.Copy(sheet);

            }
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Worksheet s = n.Worksheets[sheet.Name];
                CopyOptions copyOptions = new CopyOptions();
                copyOptions.ReferToSheetWithSameName = true;
                s.Copy(sheet, copyOptions);
            }
            Assert.AreEqual(1,n.DataConnections.Count);
            Util.ReSave(n, SaveFormat.Xlsx);
            //n.Save(Constants.destPath + &quot;CellsNet54216.xlsx&quot;);
        }
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


