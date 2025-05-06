---
title: OleObject.IsLink
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Returns true if the OleObject links to the file
type: docs
url: /net/aspose.cells.drawing/oleobject/islink/
---
## OleObject.IsLink property

Returns true if the OleObject links to the file.

```csharp
public bool IsLink { get; set; }
```

### Examples

```csharp
// Called: obj.IsLink = false;
[Test]
        public void Property_IsLink()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet44258.xls&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            OleObject oleObj = worksheet.OleObjects[0];

            byte[] pdfBytes = File.ReadAllBytes(Constants.sourcePath + &quot;CellsNet44258.pdf&quot;);

            OleObject obj = worksheet.OleObjects[0];

            obj.DisplayAsIcon = false;
            obj.FileFormatType = FileFormatType.Pdf;
            obj.ImageSourceFullName = null;
            obj.IsAutoSize = false;
            obj.IsLink = false;
            obj.ObjectData = pdfBytes;
            obj.ObjectSourceFullName = null;
            obj.ProgID = &quot;Acrobat Document&quot;;

            Util.SaveManCheck(workbook, &quot;Shape&quot;, &quot;CellsNet44258.xls&quot;);

        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


