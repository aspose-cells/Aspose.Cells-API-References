---
title: FormatCondition.IconSet
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Get the conditional formattings IconSet instance. The default instances IconSetType is TrafficLights31. Valid only for type  IconSet
type: docs
url: /net/aspose.cells/formatcondition/iconset/
---
## FormatCondition.IconSet property

Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only for type = IconSet.

```csharp
public IconSet IconSet { get; }
```

### Examples

```csharp
// Called: val = fc.IconSet.Cfvos[i].Value;
[Test]
        public void Property_IconSet()
        {
            //String filePath = Constants.destPath + &quot;Test1Conditionaldest.xlsx&quot;;
            Workbook _book = new Workbook();
            Worksheet _sheet = _book.Worksheets[0];
            //write
            FormatConditionCollection conds = GetFormatCondition(&quot;M1:O2&quot;, Color.AliceBlue, _sheet);
            int idx = conds.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = conds[idx];
            cond.IconSet.Type = IconSetType.Stars3;
            cond.IconSet.ShowValue = false;
            cond.IconSet.Reverse = true;
            Cell c = _sheet.Cells[&quot;M1&quot;];
            c.PutValue(&quot;Stars3&quot;);

           //_book.Save(filePath, SaveFormat.Xlsx);
            //read
            _book = Util.ReSave(_book, SaveFormat.Xlsx);// new Workbook(filePath);
            _sheet = _book.Worksheets[0];
            //
            FormatConditionCollection fcs = _sheet.ConditionalFormattings[0];
            FormatCondition fc = null;
            if (fcs.Count &gt; 0)
                fc = fcs[0];

            int priority;
            bool showValue, reverse;
            object val = null;
            string sqref = &quot;&quot;, fcvalue;

            FormatConditionType fcType = fc.Type;
            IconSetType iconType = fc.IconSet.Type;
            FormatConditionValueType fcvType = fc.IconSet.Cfvos[0].Type;

            priority = fc.Priority;
            showValue = fc.IconSet.ShowValue;
            reverse = fc.IconSet.Reverse;

            Assert.AreEqual(priority, 1);
            Assert.AreEqual(fcType, FormatConditionType.IconSet);
            Assert.AreEqual(iconType, IconSetType.Stars3);
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

* class [IconSet](../../iconset/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


