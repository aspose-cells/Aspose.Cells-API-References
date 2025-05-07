---
title: Enum IconSetType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.IconSetType enum. Icon set type for conditional formatting. The threshold values for triggering the different icons within a set are configurable and the icon order is reversible
type: docs
url: /net/aspose.cells/iconsettype/
---
## IconSetType enumeration

Icon set type for conditional formatting. The threshold values for triggering the different icons within a set are configurable, and the icon order is reversible.

```csharp
public enum IconSetType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Arrows3 | `0` | 3 arrows icon set. |
| ArrowsGray3 | `1` | 3 gray arrows icon set. |
| Flags3 | `2` | 3 flags icon set. |
| Signs3 | `3` | 3 signs icon set. |
| Symbols3 | `4` | 3 symbols icon set (circled). |
| Symbols32 | `5` | 3 Symbols icon set (uncircled). |
| TrafficLights31 | `6` | 3 traffic lights icon set (unrimmed). |
| TrafficLights32 | `7` | 3 traffic lights icon set with thick black border. |
| Arrows4 | `8` | 4 arrows icon set. |
| ArrowsGray4 | `9` | 4 gray arrows icon set. |
| Rating4 | `10` | 4 ratings icon set. |
| RedToBlack4 | `11` | 4 'red to black' icon set. |
| TrafficLights4 | `12` | 4 traffic lights icon set. |
| Arrows5 | `13` | 5 arrows icon set. |
| ArrowsGray5 | `14` | 5 gray arrows icon set. |
| Quarters5 | `15` | 5 quarters icon set. |
| Rating5 | `16` | 5 rating icon set. |
| Stars3 | `17` | 3 stars set |
| Boxes5 | `18` | 5 boxes set |
| Triangles3 | `19` | 3 triangles set |
| None | `20` | None |
| CustomSet | `21` | CustomSet. This element is read-only. |
| Smilies3 | `22` | 3 smilies. Only for .ods. |
| ColorSmilies3 | `23` | 3 color smilies. Only for .ods. |

### Examples

```csharp
// Called: cond.IconSet.Type = IconSetType.Stars3;
[Test]
        public void Type_IconSetType()
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


