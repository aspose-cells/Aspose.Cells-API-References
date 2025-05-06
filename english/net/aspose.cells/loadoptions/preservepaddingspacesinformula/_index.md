---
title: LoadOptions.PreservePaddingSpacesInFormula
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false
type: docs
url: /net/aspose.cells/loadoptions/preservepaddingspacesinformula/
---
## LoadOptions.PreservePaddingSpacesInFormula property

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.

```csharp
public bool PreservePaddingSpacesInFormula { get; set; }
```

### Remarks

After loading workbook from template file with this option, [`PreservePaddingSpaces`](../../formulasettings/preservepaddingspaces/) will be set to the same value with this property.

### Examples

```csharp
// Called: new LoadOptions(LoadFormat.Xlsx) { PreservePaddingSpacesInFormula = true } );
[Test]
        public void Property_PreservePaddingSpacesInFormula()
        {
            Workbook wb = new Workbook();
            wb.Settings.FormulaSettings.PreservePaddingSpaces = true;
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            string fml = &quot;= IF(1 &lt;&gt;2,2,1)&quot;;
            cell.Formula = fml;
            Assert.AreEqual(fml, cell.Formula, &quot;Parsed formula&quot;);
            wb = Util.ReSave(wb, new OoxmlSaveOptions(SaveFormat.Xlsx),
                new LoadOptions(LoadFormat.Xlsx) { PreservePaddingSpacesInFormula = true } );
            Assert.AreEqual(fml, wb.Worksheets[0].Cells[0, 0].Formula, &quot;Reloaded formula&quot;);
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


