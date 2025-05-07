---
title: PasteOptions.PasteType
second_title: Aspose.Cells for .NET API Reference
description: PasteOptions property. The paste special type
type: docs
url: /net/aspose.cells/pasteoptions/pastetype/
---
## PasteOptions.PasteType property

The paste special type.

```csharp
public PasteType PasteType { get; set; }
```

### Examples

```csharp
// Called: options.PasteType = (PasteType.All);
[Test]
        public void Property_PasteType()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsJava41807.xlsx");

           // int h = wb.Worksheets["Сводка"].Cells.Rows[0].RawHeight;
            Aspose.Cells.Range range = wb.Worksheets["Сводка"].Cells.CreateRange(0, 8, 548, 9);
            Aspose.Cells.Range source = wb.Worksheets["Сводка"].Cells.CreateRange(0, 7, 548, 7);

            PasteOptions options = new PasteOptions();
            options.PasteType = (PasteType.All);
            range.Copy(source, options);

         //   Assert.AreEqual(wb.Worksheets["Сводка"].Cells.Rows[0].RawHeight, h);
        }
```

### See Also

* enum [PasteType](../../pastetype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


