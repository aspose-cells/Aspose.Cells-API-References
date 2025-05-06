---
title: OdsSaveOptions.OdsSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: OdsSaveOptions constructor. Creates the options of saving ods file
type: docs
url: /net/aspose.cells/odssaveoptions/odssaveoptions/
---
## OdsSaveOptions() {#constructor}

Creates the options of saving ods file.

```csharp
public OdsSaveOptions()
```

### Examples

```csharp
// Called: OdsSaveOptions saveOptions = new OdsSaveOptions();
[Test]
        public void OdsSaveOptions_Constructor()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET55185.xlsx&quot;);
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.OdfStrictVersion = Aspose.Cells.Ods.OpenDocumentFormatVersionType.Odf13;
            workbook.Save(Constants.destPath + &quot;CELLSNET55185.ods&quot;, saveOptions);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET55185.ods&quot;);
            FormatConditionCollection fcs = workbook.Worksheets[0].ConditionalFormattings[0];
            CellArea ca = fcs.GetCellArea(0);
            Assert.AreEqual(ca.EndRow, 0xFFFFF);
            Assert.AreEqual(2, ca.StartColumn);
        }
```

### See Also

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsSaveOptions(SaveFormat) {#constructor_1}

Creates the options of saving ods file.

```csharp
public OdsSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be Ods, Ots, Fods or Sxc, otherwise the saved format will be set as Ods automatically. |

### See Also

* enum [SaveFormat](../../saveformat/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


