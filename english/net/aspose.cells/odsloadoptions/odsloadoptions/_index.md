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
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsNet45916.xlsx&quot;);

            wb.Save(Constants.destPath + &quot;CellsNet45916.ods&quot;);
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            loadOptions.RefreshPivotTables = true;
            wb = new Workbook(Constants.destPath + &quot;CellsNet45916.ods&quot;, loadOptions);
            wb.Save(Constants.destPath + &quot;CellsNet45916.html&quot;);
            Cell cell = wb.Worksheets[0].Cells[&quot;L20&quot;];
            Assert.AreEqual(&quot;Sports Type&quot;, cell.StringValue);
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


