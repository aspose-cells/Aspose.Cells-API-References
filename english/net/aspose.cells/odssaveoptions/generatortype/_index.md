---
title: OdsSaveOptions.GeneratorType
second_title: Aspose.Cells for .NET API Reference
description: OdsSaveOptions property. Gets and sets the generator of the ods file
type: docs
url: /net/aspose.cells/odssaveoptions/generatortype/
---
## OdsSaveOptions.GeneratorType property

Gets and sets the generator of the ods file.

```csharp
public OdsGeneratorType GeneratorType { get; set; }
```

### Examples

```csharp
// Called: saveOptions.GeneratorType = Aspose.Cells.Ods.OdsGeneratorType.LibreOffice;
[Test]
        public void Property_GeneratorType()
        {
            Style style = null;
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet46737.xlsx&quot;);
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.GeneratorType = Aspose.Cells.Ods.OdsGeneratorType.LibreOffice;
            
            workbook.Save(Constants.destPath + &quot;CellsNet46737.ods&quot;, saveOptions);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet46737.ods&quot;);
            style = workbook.Worksheets[0].Cells[&quot;B2&quot;].GetStyle();
            Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Medium);
            style = workbook.Worksheets[0].Cells[&quot;B4&quot;].GetStyle();
            Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Thick);
            style = workbook.Worksheets[0].Cells[&quot;B7&quot;].GetStyle();
            Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Double);
            workbook.Save(Constants.destPath + &quot;CellsNet46737dest.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet46737dest.xlsx&quot;);
            style = workbook.Worksheets[0].Cells[&quot;B2&quot;].GetStyle();
            Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Medium);
            style = workbook.Worksheets[0].Cells[&quot;B4&quot;].GetStyle();
            Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Thick);
            style = workbook.Worksheets[0].Cells[&quot;B7&quot;].GetStyle();
            Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Double);
        }
```

### See Also

* enum [OdsGeneratorType](../../../aspose.cells.ods/odsgeneratortype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


