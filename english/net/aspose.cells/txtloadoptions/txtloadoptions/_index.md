---
title: TxtLoadOptions.TxtLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions constructor. Creates the options for loading text file
type: docs
url: /net/aspose.cells/txtloadoptions/txtloadoptions/
---
## TxtLoadOptions() {#constructor}

Creates the options for loading text file.

```csharp
public TxtLoadOptions()
```

### Remarks

The default load file type is CSV .

### Examples

```csharp
// Called: TxtLoadOptions loadOptions = new TxtLoadOptions();
[Test]
        public void TxtLoadOptions_Constructor()
        {
            string FileName = Constants.bugFilePath + "ea.xls";
            Workbook workbook = new Workbook(FileName);
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.Separator = ',';
            workbook.Save(Constants.destPath + "testSave.CSV", saveOptions);

            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.SeparatorString = ",";
            workbook = new Workbook(Constants.destPath + "testSave.CSV", loadOptions);
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtLoadOptions(LoadFormat) {#constructor_1}

Creates the options for loading text file.

```csharp
public TxtLoadOptions(LoadFormat loadFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loading format |

### See Also

* enum [LoadFormat](../../loadformat/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


