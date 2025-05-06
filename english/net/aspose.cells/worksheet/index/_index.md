---
title: Worksheet.Index
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the index of sheet in the worksheet collection
type: docs
url: /net/aspose.cells/worksheet/index/
---
## Worksheet.Index property

Gets the index of sheet in the worksheet collection.

```csharp
public int Index { get; }
```

### Examples

```csharp
// Called: cellEnum = source.Worksheets[sheet.Index].Cells.GetEnumerator();
public bool Property_Index(Worksheet sheet)
            {
                processed |= 0x01;
                //checking apis
                sheet.Workbook.Settings.ShowTabs = true;
                if (sheetName != null &amp;&amp; !sheet.Name.ToUpper().Equals(sheetName))
                {
                    Console.WriteLine(&quot;Ignore sheet[&quot; + sheet.Index + &quot;][&quot; + sheet.Name + &quot;]&quot;);
                    return false;
                }
                currSheet = sheet;
                Console.WriteLine(&quot;Processing sheet[&quot; + sheet.Index + &quot;][&quot; + sheet.Name + &quot;]&quot;);
                if (startRow &lt; 0)
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

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


