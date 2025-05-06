---
title: FontSetting.Font
second_title: Aspose.Cells for .NET API Reference
description: FontSetting property. Returns the font of this object
type: docs
url: /net/aspose.cells/fontsetting/font/
---
## FontSetting.Font property

Returns the font of this object.

```csharp
public Font Font { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(fs.Font.Size, 8);
[Test]
        public void Property_Font()
        {
            
 String [] columnText = 
			{
				/* campaign decomp */ 	&quot;This column addresses whether the variable being measured is representative of the total campaign or only a part or decomposition of the total.&quot;,
				/* campaign var */ 			&quot;The aspect of the campaign being measured. Typically it is an individual creative or audience part, broken out by an attribute previously determined in the SOW.&quot;,
				/* net dollar eff */ 			&quot;Measures the net dollars spent on the brand among each confirmed category purchase occasion.\n\nThe higher the number, the better the variable is performing relative to all the other variables. If the number is above 100, the variable is performing better than the average of all variables.&quot;,
				/* current % distr */ 			&quot;This column, reported as a percent, indicates the current distribution of impressions being received by NCS and counted in InFlight for each variable as a percent of the total distribution. &quot;,
				/* impress deliv */ 			&quot;The values in this column report the number of impressions observed for each variable within the exposure window between the start and end dates indicated in the fifth and sixth rows of the report, and the total number of impressions delivered over the life of the report.&quot;,
				/* est min impress */			&quot;This value indicates approximately what amount of impressions must be delivered through each variable so that it will deliver the minimum number of exposed brand purchase occasions (50) required for it to contribute to the effectiveness indices.\n\nThis is calculated as:\nCurrent Impressions Delivered divided by (Exposed Purchases / 50)\n\nPurchases are counted when a household that was exposed to the tactic, within the exposure window, was likely to have purchased the brand as a result of having been exposed.&quot;			
			};
            Workbook workbook = new Workbook();
            Worksheet weekEndingWS = workbook.Worksheets[0];
        int [] colMap = {0, 1, 2, 4, 6, 8};	// used to get the real position of the merged cells

            int row = 1;
        for(int col = 0; col &lt; 6; col++)
        {
			// add the comment for the column
			Comment comment = weekEndingWS.Comments[weekEndingWS.Comments.Add(row, colMap[col])];
			Aspose.Cells.Font cFont = comment.Font;
			cFont.Size=(8);
			cFont.IsBold=(false);
	
			comment.Note = (columnText[col]);
			comment.AutoSize=(false);
			comment.HeightInch=(3);
			comment.WidthInch=(2);
                FontSetting[] settings = comment.GetRichFormattings();
            foreach (FontSetting fs in settings)
            {
                Assert.AreEqual(fs.Font.Name, &quot;Tahoma&quot;);
                Assert.AreEqual(fs.Font.Size, 8);
            }
        }

        workbook.Save(Constants.destPath + &quot;CELLSJAVA42213.xlsx&quot;); 

        }
```

### See Also

* class [Font](../../font/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


