---
title: PasteOptions.SkipBlanks
second_title: Aspose.Cells for .NET API Reference
description: PasteOptions property. Indicates whether skips blank cells
type: docs
url: /net/aspose.cells/pasteoptions/skipblanks/
---
## PasteOptions.SkipBlanks property

Indicates whether skips blank cells.

```csharp
public bool SkipBlanks { get; set; }
```

### Examples

```csharp
// Called: destinationRange.Copy(sourceRange, new PasteOptions { SkipBlanks = false, PasteType = PasteType.All });
[Test]
        public void Property_SkipBlanks()
        {
            Workbook Source = new Workbook(Constants.sourcePath + &quot;Copy/N46671_S.xlsx&quot;);
            Workbook Destination = new Workbook(Constants.sourcePath + &quot;Copy/N46671_D.xlsx&quot;);
            Aspose.Cells.Range sourceRange = Source.Worksheets.GetRangeByName(&quot;Range1&quot;);
            Worksheet targetSheet = Destination.Worksheets[0];
            Aspose.Cells.Range destinationRange = targetSheet.Cells.CreateRange(3, 25, sourceRange.RowCount, sourceRange.ColumnCount);
            destinationRange.CopyData(sourceRange);
            destinationRange.Copy(sourceRange, new PasteOptions { SkipBlanks = false, PasteType = PasteType.All });
            Util.ReSave(Destination, SaveFormat.Xlsx);
        }
```

### See Also

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


