---
title: StyleFlag.WrapText
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Wrap text setting will be applied
type: docs
url: /net/aspose.cells/styleflag/wraptext/
---
## StyleFlag.WrapText property

Wrap text setting will be applied.

```csharp
public bool WrapText { get; set; }
```

### Examples

```csharp
// Called: sheet.Cells.ApplyStyle(style, new StyleFlag() { WrapText = true });
[Test]
        public void Property_WrapText()
        {
            Workbook wb = new Workbook(Constants.sourcePath +&quot;iteration-car_init-CountNums.xls&quot;);
            Worksheet sheet = wb.Worksheets[0];
            string outputPath = Constants.destPath;

            // Get list of groups

            // Set up conditional formatting for subtotal rows
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            int colCompValue = 0;

            for (int i = 0; i &lt; 2; i++)
            {
                //    wb.Save(String.Format(@&quot;{1}output_{0}_pre-subtotal.xls&quot;, i * 3, outputPath), SaveFormat.Excel97To2003); //////////////////////////////////////////////////////

                CellArea ca = new CellArea()
                {
                    StartRow = 4,
                    StartColumn = 0,
                    EndRow = sheet.Cells.MaxDataRow,
                    EndColumn = sheet.Cells.MaxDataColumn
                };
                sheet.Cells.Subtotal(ca, i + colCompValue, ConsolidationFunction.CountNums, new int[] { 1 }, false, false, true);
                //int conditionIndex = fcs.AddCondition(FormatConditionType.Expression);
                //FormatCondition fc = fcs[conditionIndex];
                //string searchName = &quot;MIN&quot;;
                //fc.Formula1 = String.Format(@&quot;=RIGHT(${0}{1},{2})=&quot;&quot;{3}&quot;&quot;&quot;, (char)(i + (int)&apos;A&apos;), 5, searchName.Length, searchName);
                //fc.Style = new Style() { BackgroundColor = System.Drawing.Color.FromArgb(159, 191, 213) };
                wb.Save(String.Format(@&quot;{1}output_{0}_MAX_subtotal.xls&quot;, i * 3 + 1, outputPath), SaveFormat.Excel97To2003); ////////////////////////////////////////////
            }

            // Set the area for the conditional formatting rules
            CellArea caData = new CellArea()
            {
                StartRow = 4,
                StartColumn = 0,
                EndRow = sheet.Cells.MaxDataRow,
                EndColumn = sheet.Cells.MaxDataColumn
            };
            if (fcs.Count &gt; 0) { fcs.AddArea(caData); }

            var style = wb.CreateStyle();
            style.IsTextWrapped = false;

            sheet.Cells.ApplyStyle(style, new StyleFlag() { WrapText = true });

            wb.Save(outputPath + &quot;CellsNet40800.xls&quot;);
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


