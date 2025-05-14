---
title: TxtSaveOptions.TxtSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions constructor. Creates text file save options
type: docs
url: /net/aspose.cells/txtsaveoptions/txtsaveoptions/
---
## TxtSaveOptions() {#constructor}

Creates text file save options.

```csharp
public TxtSaveOptions()
```

### Examples

```csharp
// Called: TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
[Test, Category("Bug")]
        public void TxtSaveOptions_Constructor()
        {
            Workbook workbook = new Workbook();
            //workbook.Open(Constants.sourcePath + "string-seperated.txt", "*#*");
            //workbook.SaveToCSV(Constants.destPath +"Test_29205.txt", "*#*");
            TxtLoadOptions txtLoadOption = new TxtLoadOptions();
            txtLoadOption.SeparatorString = "*#*";
            workbook = new Workbook(Constants.sourcePath + "string-seperated.txt", txtLoadOption);
            TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
            txtSaveOptions.SeparatorString = "*#*";
            workbook.Save(Constants.destPath + "Test_29205.txt", txtSaveOptions);
        }
```

### See Also

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtSaveOptions(SaveFormat) {#constructor_1}

Creates text file save options.

```csharp
public TxtSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be Csv or Tsv, otherwise the saved format will be set as Csv automatically. |

### See Also

* enum [SaveFormat](../../saveformat/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


