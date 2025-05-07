---
title: Range.ToHtml
second_title: Aspose.Cells for .NET API Reference
description: Range method. Convert the range to html 
type: docs
url: /net/aspose.cells/range/tohtml/
---
## Range.ToHtml method

Convert the range to html .

```csharp
public byte[] ToHtml(HtmlSaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | HtmlSaveOptions | Options for coverting range to html. |

### Examples

```csharp
// Called: byte[] htmlData = r.ToHtml(null);
[Test]
        public void Method_HtmlSaveOptions_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET55578.xlsx");
            //A1:J25
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range r = cells.CreateRange("A1:J25");
            byte[] data = r.ToImage(null);

            byte[] htmlData = r.ToHtml(null);
            string json = r.ToJson(null);
        }
```

### See Also

* class [HtmlSaveOptions](../../htmlsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


