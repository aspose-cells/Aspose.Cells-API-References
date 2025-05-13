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
public void Workbook_Method_Copy()
{
    var workbook1 = new Workbook(Constants.sourcePath + @"example.xlsm");
           
    var workbook2 = new Workbook(Constants.sourcePath + @"example.xlsx");
    CopyOptions options = new CopyOptions();
    options.KeepMacros = true;
    workbook1.Copy(workbook2, options);
    Assert.AreEqual(1,workbook1.VbaProject.Modules.Count);
    workbook1.Save(Constants.destPath + "example.xlsm");
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
// Called: workbook2.Copy(workbook);
public void Workbook_Method_Copy()
{
    Console.WriteLine("Workbook_Method_Copy()");
    string infn = path + "TEST_KeepShapeCopy.xlsm";
    string outfn = Constants.destPath + "TEST_KeepShapeCopy_out.xlsx";

    Workbook workbook = new Workbook(infn);
    Workbook workbook2 = new Workbook();
    workbook2.Copy(workbook);
    workbook2.Save(outfn);
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


