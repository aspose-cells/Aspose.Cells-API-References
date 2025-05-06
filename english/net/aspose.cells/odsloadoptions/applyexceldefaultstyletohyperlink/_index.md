---
title: OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink
second_title: Aspose.Cells for .NET API Reference
description: OdsLoadOptions property. Indicates whether applying the default style of the Excel to hyperlink
type: docs
url: /net/aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink/
---
## OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink property

Indicates whether applying the default style of the Excel to hyperlink.

```csharp
public bool ApplyExcelDefaultStyleToHyperlink { get; set; }
```

### Examples

```csharp
// Called: loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
[Test]
        public void Property_ApplyExcelDefaultStyleToHyperlink()
        {
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA42798.ods&quot;, loadOptions);
            workbook.Save(Constants.destPath + &quot;CELLSJAVA42798.xlsx&quot;);
            AssertHelper.AreEqual(workbook.Worksheets[0].Cells[&quot;B1&quot;].GetStyle().Font.Color, Color.Blue);
            

        }
```

### See Also

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


