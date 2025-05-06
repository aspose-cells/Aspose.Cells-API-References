---
title: Picture.Formula
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Gets and sets the data of the formula
type: docs
url: /net/aspose.cells.drawing/picture/formula/
---
## Picture.Formula property

Gets and sets the data of the formula.

```csharp
public string Formula { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;=B1:B3&amp;quot;, workbook.Worksheets[0].Pictures[0].Formula);
[Test]
          public void Property_Formula()
          {
              Workbook workbook = new Workbook();
              Picture picture = workbook.Worksheets[0].Pictures[workbook.Worksheets[0].Pictures.Add(0, 0, Constants.sourcePath + &quot;417_Eni_versalis.jpg&quot;)];
              picture.Formula = &quot;A1:A3&quot;;
              workbook.Save(Constants.destPath + &quot;CELLSNET44709.xls&quot;);
              workbook = new Workbook(Constants.destPath + &quot;CELLSNET44709.xls&quot;);
              Assert.AreEqual(&quot;=A1:A3&quot;, workbook.Worksheets[0].Pictures[0].Formula);

              workbook.Worksheets[0].Pictures[0].Formula = &quot;B1:B3&quot;;
              workbook.Save(Constants.destPath + &quot;CELLSNET44709.xls&quot;);
              workbook = new Workbook(Constants.destPath + &quot;CELLSNET44709.xls&quot;);
              Assert.AreEqual(&quot;=B1:B3&quot;, workbook.Worksheets[0].Pictures[0].Formula);
          }
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


