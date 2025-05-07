---
title: Worksheet.Workbook
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the workbook object which contains this sheet
type: docs
url: /net/aspose.cells/worksheet/workbook/
---
## Worksheet.Workbook property

Gets the workbook object which contains this sheet.

```csharp
public Workbook Workbook { get; }
```

### Examples

```csharp
// Called: sheet.Workbook.Settings.ShowTabs = true;
public bool Property_Workbook(Worksheet sheet)
            {
                processed |= 0x01;
                //checking apis
                sheet.Workbook.Settings.ShowTabs = true;
                if (sheetName != null && !sheet.Name.ToUpper().Equals(sheetName))
                {
                    Console.WriteLine("Ignore sheet[" + sheet.Index + "][" + sheet.Name + "]");
                    return false;
                }
                currSheet = sheet;
                Console.WriteLine("Processing sheet[" + sheet.Index + "][" + sheet.Name + "]");
                if (startRow < 0)
                {
                    cellEnum = source.Worksheets[sheet.Index].Cells.GetEnumerator();
                }
                else
                {
                    cellEnum = source.Worksheets[sheet.Index].Cells.CreateRange(startRow, startCol, endRow - startRow + 1, endCol - startCol + 1).GetEnumerator();
                }
                firstSheetErr = true;
                return true;
            }
```

### See Also

* class [Workbook](../../workbook/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


