---
title: Cell.Column
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets column number zero based of the cell
type: docs
url: /net/aspose.cells/cell/column/
---
## Cell.Column property

Gets column number (zero based) of the cell.

```csharp
public int Column { get; }
```

### Examples

```csharp
// Called: Cell cellDest = cellsDest.CheckCell(cellSrc.Row, cellSrc.Column);
public static void Property_Column(Workbook workbookSrc, Workbook workbookDest,  CompareOption option)
        {
            if (option.WorkbookProperty)
            {
                CompareWorkbookProperty(workbookSrc, workbookDest);
            }

            if (option.BuiltInProperty)
            {
                BuiltInDocumentPropertyCollection bp1 = workbookSrc.BuiltInDocumentProperties;
                BuiltInDocumentPropertyCollection bp2 = workbookDest.BuiltInDocumentProperties;
                CompareBuiltInProperty(&quot;Workbook &quot;, bp1, bp2);
                //Write2Txt(bp1, bp2);
            }

            if (option.CustomProperty)
            {
                CustomDocumentPropertyCollection cp1 = workbookSrc.CustomDocumentProperties;
                CustomDocumentPropertyCollection cp2 = workbookDest.CustomDocumentProperties;
                CompareCustomProperty(cp1, cp2);
            }

            for (int sheetIndex = 0; sheetIndex &lt; workbookSrc.Worksheets.Count; sheetIndex++)
            {
                Worksheet worksheetSrc = workbookSrc.Worksheets[sheetIndex];
                Worksheet worksheetDest = workbookDest.Worksheets[sheetIndex];
                if (option.WorksheetProperty)
                {
                    CompareWorksheetProperty(worksheetSrc.Name, worksheetSrc, worksheetDest);
                }

                if (option.PageSetupProperty)
                {
                    PageSetup pageSetupSrc = worksheetSrc.PageSetup;
                    PageSetup pageSetupDest = worksheetDest.PageSetup;
                    ComparePageSetupProperty(worksheetSrc.Name, pageSetupSrc, pageSetupDest);
                }

                if (option.AutoFilterProperty)
                {
                    AutoFilter autoFilter1 = worksheetSrc.AutoFilter;
                    AutoFilter autoFilter2 = worksheetDest.AutoFilter;
                    CompareAutoFilterProperty(&quot;!&quot; + worksheetSrc.Name + &quot;--AutoFilter:&quot;, autoFilter1, autoFilter2);
                }

                if (option.HyperlinkProperty)
                {
                    HyperlinkCollection hyperlinks1 = worksheetSrc.Hyperlinks;
                    HyperlinkCollection hyperlinks2 = worksheetSrc.Hyperlinks;
                    for (int hlIndex = 0; hlIndex &lt; hyperlinks1.Count; hlIndex++)
                    {
                        Hyperlink hyperlink1 = hyperlinks1[hlIndex];
                        Hyperlink hyperlink2 = hyperlinks2[hlIndex];
                        CompareHyperlinkProperty(worksheetSrc.Name, hyperlink1, hyperlink2);
                    }
                }

                if (option.ConditionFormatProperty)
                {
                    ConditionalFormattingCollection cfc1 = worksheetSrc.ConditionalFormattings;
                    ConditionalFormattingCollection cfc2 = worksheetDest.ConditionalFormattings;
                    CompareConditionFormatProperty(worksheetSrc.Name, cfc1, cfc2);
                }

                Cells cellsSrc = worksheetSrc.Cells;
                Cells cellsDest = worksheetDest.Cells;

                foreach (Cell cellSrc in cellsSrc)
                {
                    Cell cellDest = cellsDest.CheckCell(cellSrc.Row, cellSrc.Column);
                    if (option.CellValue)
                    {
                        CompareCellValue(cellSrc, cellDest, option.IsHtm);
                    }
                    if (option.CellProperty)
                    {
                        CompareCellValue(cellSrc, cellDest, option.IsHtm);
                        CompareCellProperty(worksheetSrc.Name, cellSrc, cellDest);
                    }
                    if (option.CellRotation)
                    {
                        CompareCellRotation(cellSrc, cellDest);
                    }
                    if (option.Style)
                    {
                        Style styleSrc = cellSrc.GetStyle();
                        Style styleDest = cellDest.GetStyle();
                        CompareStyle.compareStyle(worksheetSrc.Name + &quot;!&quot; + cellSrc.Name + &quot;:&quot;, styleSrc, styleDest);
                    }
                }
            }
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


