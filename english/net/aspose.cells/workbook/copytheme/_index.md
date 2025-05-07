---
title: Workbook.CopyTheme
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Copies the theme from another workbook
type: docs
url: /net/aspose.cells/workbook/copytheme/
---
## Workbook.CopyTheme method

Copies the theme from another workbook.

```csharp
public void CopyTheme(Workbook source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | Source workbook. |

### Examples

```csharp
// Called: targetWorkbook.CopyTheme(sourceWorkbook);
[Test]
        public void Method_Workbook_()
        {
            Workbook sourceWorkbook = new Workbook(Constants.sourcePath + "CellsJava42848.xlsx");
            Cells sourcCells = sourceWorkbook.Worksheets[3].Cells;
            Aspose.Cells.Range sourceRange = sourcCells.CreateRange("A1", "P10");

            Workbook targetWorkbook = new Workbook();
            targetWorkbook.CopyTheme(sourceWorkbook);
            targetWorkbook.DefaultStyle = (sourceWorkbook.DefaultStyle);

            Cells targetCells = targetWorkbook.Worksheets[0].Cells;
            Aspose.Cells.Range targetRange = targetCells.CreateRange("A1", "P10");

            PasteOptions pasteOptions = new PasteOptions();
            // pasteOptions.setPasteType(PasteType.COLUMN_WIDTHS + PasteType.ROW_HEIGHTS + PasteType.FORMATS + PasteType.VALUES_AND_NUMBER_FORMATS);
            pasteOptions.PasteType = (PasteType.All);

            targetRange.Copy(sourceRange, pasteOptions);

            // Save the Excel file
            targetWorkbook.Save(Constants.destPath + "CellsJava42848.xlsx");
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


