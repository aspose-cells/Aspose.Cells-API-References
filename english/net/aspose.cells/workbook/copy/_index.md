---
title: Workbook.Copy
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Copies another Workbook object
type: docs
url: /net/aspose.cells/workbook/copy/
---
## Copy(Workbook, CopyOptions) {#copy_1}

Copies another Workbook object.

```csharp
public void Copy(Workbook source, CopyOptions copyOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | Source Workbook object. |
| copyOptions | CopyOptions | The options of copying other workbook. |

### Remarks

It's very simple to clone an Excel file.

### Examples

```csharp
// Called: workbook1.Copy(workbook2, options);
[Test]
        public void Method_CopyOptions_()
        {
            var workbook1 = new Workbook(Constants.sourcePath + @"CellsNet47570.xlsm");
           
            var workbook2 = new Workbook(Constants.sourcePath + @"CellsNet47570.xlsx");
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;
            workbook1.Copy(workbook2, options);
            Assert.AreEqual(1,workbook1.VbaProject.Modules.Count);
            workbook1.Save(Constants.destPath + "CellsNet47570.xlsm");
        }
```

### See Also

* class [CopyOptions](../../copyoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Workbook) {#copy}

Copies data from a source Workbook object.

```csharp
public void Copy(Workbook source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | Source Workbook object. |

### Examples

```csharp
// Called: copy.Copy(wb);
[Test]
        public void Method_Workbook_()
        {
            //test.CellsNet46949();
            LoadOptions options = new LoadOptions();
            options.AutoFitterOptions = new AutoFitterOptions();
            options.AutoFitterOptions.OnlyAuto = true;
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSJAVA-42180.xlsx", options);
            Assert.AreEqual(wb.Worksheets[0].Cells.StandardHeight,15);
            Workbook copy = new Workbook();
            copy.Copy(wb);
            Assert.AreEqual(copy.Worksheets[0].Cells.StandardHeight,15);
            wb.Save(Constants.destPath + "CellsJava42180.xlsx");
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


