---
title: IconSet.ShowValue
second_title: Aspose.Cells for .NET API Reference
description: IconSet property. Get or set the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true
type: docs
url: /net/aspose.cells/iconset/showvalue/
---
## IconSet.ShowValue property

Get or set the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true.

```csharp
public bool ShowValue { get; set; }
```

### Examples

```csharp
// Called: showValue = fc.IconSet.ShowValue;
[Test]
        public void Property_ShowValue()
        {

            //String filePath = Constants.destPath + &quot;Test2Conditionaldest.xlsx&quot;;
            Workbook _book = new Workbook();
            Worksheet _sheet = _book.Worksheets[0];
            //write
            FormatConditionCollection conds = GetFormatCondition(&quot;M1:O2&quot;, Color.AliceBlue, _sheet);
            int idx = conds.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = conds[idx];
            cond.IconSet.Type = IconSetType.Triangles3;
            cond.IconSet.ShowValue = false;
            cond.IconSet.Reverse = true;
            Cell c = _sheet.Cells[&quot;M1&quot;];
            c.PutValue(&quot;Triangles3&quot;);

            //_book.Save(filePath, SaveFormat.Xlsx);
            //read
            _book = Util.ReSave(_book, SaveFormat.Xlsx);// new Workbook(filePath);
            _sheet = _book.Worksheets[0];
            //
            FormatConditionCollection fcs = _sheet.ConditionalFormattings[0];
            FormatCondition fc = null;
            if (fcs.Count &gt; 0)
                fc = fcs[0];
            string fcvalue = &quot;&quot;;
            int priority;
            object val = null;
            string sqref = &quot;&quot;;
            bool showValue, reverse;

            FormatConditionType fcType = fc.Type;
            IconSetType iconType = fc.IconSet.Type;
            FormatConditionValueType fcvType = fc.IconSet.Cfvos[0].Type;

            priority = fc.Priority;
            showValue = fc.IconSet.ShowValue;
            reverse = fc.IconSet.Reverse;
            Assert.AreEqual(priority, 1);
            Assert.AreEqual(fcType, FormatConditionType.IconSet);
            Assert.AreEqual(iconType, IconSetType.Triangles3);
            Assert.AreEqual(fcvType, FormatConditionValueType.Percent);
            int count = fc.IconSet.Cfvos.Count;
            string[] vals = new string[] { &quot;0&quot;, &quot;33&quot;, &quot;67&quot; };
            for (int i = 0; i &lt; count; i++)
            {
                val = fc.IconSet.Cfvos[i].Value;
                fcvalue = val.ToString();
                Assert.AreEqual(fcvalue, vals[i]);
            }
            Assert.AreEqual(showValue, false);
            Assert.AreEqual(reverse, true);
            CellArea cellare = fcs.GetCellArea(0);
            sqref = GetCellAreaName(cellare);
            Assert.AreEqual(sqref, &quot;M1:O2&quot;);
        }
```

### See Also

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


