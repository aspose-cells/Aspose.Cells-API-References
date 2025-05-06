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
// Called: TxtSaveOptions saveOptions = new TxtSaveOptions();
[Test]
        public void TxtSaveOptions_Constructor()
        {
            string FileName = Constants.sourcePath + &quot;TestWorkbook\\Book1.xls&quot;;
            Workbook workbook = new Workbook(FileName);
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.SeparatorString = &quot;&amp;^&quot;;
            workbook.Save(Constants.destPath + &quot;testSave.CSV&quot;, saveOptions);

            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.SeparatorString = &quot;&amp;^&quot;;
            workbook = new Workbook(Constants.destPath + &quot;testSave.CSV&quot;, loadOptions);
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


