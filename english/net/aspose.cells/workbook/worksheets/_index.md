---
title: Workbook.Worksheets
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets the WorksheetCollection collection in the spreadsheet
type: docs
url: /net/aspose.cells/workbook/worksheets/
---
## Workbook.Worksheets property

Gets the [`WorksheetCollection`](../../worksheetcollection/) collection in the spreadsheet.

```csharp
public WorksheetCollection Worksheets { get; }
```

### Return Value

[`WorksheetCollection`](../../worksheetcollection/) collection

### Examples

```csharp
// Called: wb.Worksheets[0].Cells[&amp;quot;a7&amp;quot;].Formula = &amp;quot;=Sum(T1:Y11) / 2 * ABS(Y1)&amp;quot;;
[Test, Category(&quot;Bug&quot;)]
		public void Property_Worksheets()
		{
			Workbook wb = new Workbook();
			wb.Worksheets[0].Cells[&quot;a1&quot;].Formula = &quot;=\&quot;Prospect Number - \&quot;&amp;IF(\&quot;1\&quot;=\&quot;\&quot;,\&quot;&lt;All Prospects&gt;\&quot;,\&quot;1\&quot;)&quot;;
			wb.Worksheets[0].Cells[&quot;A2&quot;].Formula = &quot;=\&quot;Action Due between \&quot;&amp;IF(\&quot;\&quot;=\&quot;\&quot;,\&quot;&lt;Any Date&gt;\&quot;,\&quot;\&quot;)&amp;\&quot; and \&quot;&amp;IF(\&quot;\&quot;=\&quot;\&quot;,\&quot;&lt;Any Date&gt;\&quot;,\&quot;\&quot;)&quot;;
			wb.Worksheets[0].Cells[&quot;A3&quot;].Formula = &quot;=\&quot;some text (\&quot;\&quot; &amp; B4 &amp; \&quot;\&quot;)\&quot;&quot;;
			wb.Worksheets.Add();
			wb.Worksheets.Add();
			wb.Worksheets.Add();
			wb.Worksheets[3].Name = &quot;IMES++ SPAR Overview Report&quot;;
			wb.Worksheets[1].Name = &quot;Balance Sheet&quot;;
			wb.Worksheets[2].Name = &quot;Model Inputs&quot;;
			wb.Worksheets[1].Cells[&quot;e15&quot;].PutValue(1);
			wb.Worksheets[2].Cells[&quot;C40&quot;].PutValue(12);
			wb.Worksheets[0].Cells[&quot;F9&quot;].PutValue(0.5);

			Cell cell = wb.Worksheets[0].Cells[&quot;A4&quot;];
			cell.Formula = @&quot;=(&apos;Balance Sheet&apos;!E15+&apos;Balance Sheet&apos;!E17+&apos;Balance Sheet&apos;!E18)/&apos;Model Inputs&apos;!C40*(1+F9)&quot;;
			
			cell = wb.Worksheets[0].Cells[&quot;A5&quot;];
			cell.Formula = &quot;=IF(FALSE, 0, 1)&quot;;
			wb.Worksheets[0].Cells[&quot;a6&quot;].Formula = &quot;=MIN(A1:A5) &amp; \&quot; | \&quot; &amp; MAX(A1:A5)&quot;;
			wb.Worksheets[0].Cells[&quot;a7&quot;].Formula = &quot;=Sum(T1:Y11) / 2 * ABS(Y1)&quot;;
			wb.Worksheets[0].Cells[&quot;A8&quot;].Formula = &quot;=\&quot;some text (\&quot; &amp; B4 &amp; \&quot;)\&quot;&quot;;
			wb.Worksheets[0].Cells[&quot;a9&quot;].Formula = &quot;=IF(A4&gt;0, ROUND(A4/A5*100,2), 0)&quot;;
			wb.Worksheets[0].Cells[&quot;A10&quot;].Formula = &quot;= - a9&quot;;
			wb.Worksheets[0].Cells[&quot;A11&quot;].Formula = &quot;=\&quot;Prospect Number - \&quot;&amp;IF(\&quot;\&quot;=\&quot;\&quot;,\&quot;&lt;All Prospects&gt;\&quot;,\&quot;\&quot;)&quot;;
			wb.Worksheets[0].Cells[&quot;A12&quot;].Formula = &quot;=SUM(A1:OFFSET(A3,-2,,))&quot;;
			wb.Worksheets[0].Cells[&quot;A13&quot;].Formula = &quot;=COUNTIF(&apos;IMES++ SPAR Overview Report&apos;!G2:G779,\&quot;Estimated\&quot;)&quot;;
			cell = wb.Worksheets[0].Cells[&quot;I9&quot;];
			cell.SetArrayFormula(&quot;=SUM(IF($A$10:$A$13=4,IF($I$10:$I$13&lt;&gt;\&quot;\&quot;,IF($F$10:$F$13&lt;&gt;-1,$I$10:$I$13*$D$10:$D$13,0),0),0))*$D9&quot;,1,1);

            wb = Util.ReSave(wb, SaveFormat.Excel97To2003);
		}
```

### See Also

* class [WorksheetCollection](../../worksheetcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


