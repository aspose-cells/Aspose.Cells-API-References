---
title: OdsLoadOptions.OdsLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: OdsLoadOptions constructor. Represents the options of loading ods file
type: docs
url: /net/aspose.cells/odsloadoptions/odsloadoptions/
---
## OdsLoadOptions() {#constructor}

Represents the options of loading ods file.

```csharp
public OdsLoadOptions()
```

### Examples

```csharp
// Called: OdsLoadOptions loadOptions = new OdsLoadOptions();
[Test]
        public void OdsLoadOptions_Constructor()
        {
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA42798.ods", loadOptions);
            workbook.Save(Constants.destPath + "CELLSJAVA42798.xlsx");
            AssertHelper.AreEqual(workbook.Worksheets[0].Cells["B1"].GetStyle().Font.Color, Color.Blue);
            

        }
```

### See Also

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsLoadOptions(LoadFormat) {#constructor_1}

Represents the options of loading ods file.

```csharp
public OdsLoadOptions(LoadFormat type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | LoadFormat | The load format type. |

### See Also

* enum [LoadFormat](../../loadformat/)
* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


