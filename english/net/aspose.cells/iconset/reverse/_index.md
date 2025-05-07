---
title: IconSet.Reverse
second_title: Aspose.Cells for .NET API Reference
description: IconSet property. Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false
type: docs
url: /net/aspose.cells/iconset/reverse/
---
## IconSet.Reverse property

Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false.

```csharp
public bool Reverse { get; set; }
```

### Examples

```csharp
// Called: reverse = fc.IconSet.Reverse;
[Test]
        public void Property_Reverse()
        {
            //String filePath = Constants.destPath + "Test1Conditionaldest.xlsx";
            Workbook _book = new Workbook();
            Worksheet _sheet = _book.Worksheets[0];
            //write
            FormatConditionCollection conds = GetFormatCondition("M1:O2", Color.AliceBlue, _sheet);
            int idx = conds.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = conds[idx];
            cond.IconSet.Type = IconSetType.Stars3;
            cond.IconSet.ShowValue = false;
            cond.IconSet.Reverse = true;
            Cell c = _sheet.Cells["M1"];
            c.PutValue("Stars3");

           //_book.Save(filePath, SaveFormat.Xlsx);
            //read
            _book = Util.ReSave(_book, SaveFormat.Xlsx);// new Workbook(filePath);
            _sheet = _book.Worksheets[0];
            //
            FormatConditionCollection fcs = _sheet.ConditionalFormattings[0];
            FormatCondition fc = null;
            if (fcs.Count > 0)
                fc = fcs[0];

            int priority;
            bool showValue, reverse;
            object val = null;
            string sqref = "", fcvalue;

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
            string[] vals = new string[] { "0", "33", "67" };
            for (int i = 0; i < count; i++)
            {
                val = fc.IconSet.Cfvos[i].Value;
                fcvalue = val.ToString();
                Assert.AreEqual(fcvalue, vals[i]);
            }
            Assert.AreEqual(showValue, false);
            Assert.AreEqual(reverse, true);
            CellArea cellare = fcs.GetCellArea(0);
            sqref = GetCellAreaName(cellare);
            Assert.AreEqual(sqref, "M1:O2");

        }
```

### See Also

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


