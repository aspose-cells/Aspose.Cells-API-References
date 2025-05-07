---
title: Border.LineStyle
second_title: Aspose.Cells for .NET API Reference
description: Border property. Gets or sets the cell border type
type: docs
url: /net/aspose.cells/border/linestyle/
---
## Border.LineStyle property

Gets or sets the cell border type.

```csharp
public CellBorderType LineStyle { get; set; }
```

### Examples

```csharp
// Called: CellBorderType beforeC13 = c13.GetStyle().Borders[BorderType.TopBorder].LineStyle;
[Test]
        public void Property_LineStyle()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET42878_";
            Workbook workbook = new Workbook(filePath + "PivotReports.xls");
            Cell c13 = workbook.Worksheets["PivotTable"].Cells["C13"];
            CellBorderType beforeC13 = c13.GetStyle().Borders[BorderType.TopBorder].LineStyle;
            Console.WriteLine("C13 top border:" + beforeC13);
            Console.WriteLine("after calculating");
            workbook.Save(Constants.PivotTableDestPath + "NET42878.xlsx");
            workbook.Worksheets["PivotTable"].PivotTables[0].CalculateData();
       
            Console.WriteLine("C13 top border:" + c13.GetStyle().Borders[BorderType.TopBorder].LineStyle);
            Assert.AreEqual(beforeC13, c13.GetStyle().Borders[BorderType.TopBorder].LineStyle);
            Color c6BeforeColor = workbook.Worksheets["PivotTable"].Cells["C6"].GetStyle().ForegroundColor;
            Assert.AreEqual(c6BeforeColor.R, 255);
            Assert.AreEqual(c6BeforeColor.G, 153);
            Assert.AreEqual(c6BeforeColor.B, 204);
            workbook.Save(Constants.PivotTableDestPath + @"NET42878.pdf");
        }
```

### See Also

* enum [CellBorderType](../../cellbordertype/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


