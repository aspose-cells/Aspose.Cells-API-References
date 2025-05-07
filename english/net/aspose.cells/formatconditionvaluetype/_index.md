---
title: Enum FormatConditionValueType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.FormatConditionValueType enum. Condition value type
type: docs
url: /net/aspose.cells/formatconditionvaluetype/
---
## FormatConditionValueType enumeration

Condition value type.

```csharp
public enum FormatConditionValueType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Formula | `0` | The minimum/ midpoint / maximum value for the gradient is determined by a formula. |
| Max | `1` | Indicates that the maximum value in the range shall be used as the maximum value for the gradient. |
| Min | `2` | Indicates that the minimum value in the range shall be used as the minimum value for the gradient. |
| Number | `3` | Indicates that the minimum / midpoint / maximum value for the gradient is specified by a constant numeric value. |
| Percent | `4` | Value indicates a percentage between the minimum and maximum values in the range shall be used as the minimum / midpoint / maximum value for the gradient. |
| Percentile | `5` | Value indicates a percentile ranking in the range shall be used as the minimum / midpoint / maximum value for the gradient. |
| AutomaticMax | `6` | Indicates that the Automatic maximum value in the range shall be used as the Automatic maximum value for the gradient. |
| AutomaticMin | `7` | Indicates that the Automatic minimum value in the range shall be used as the Automatic minimum value for the gradient. |

### Examples

```csharp
// Called: Assert.AreEqual(valueType2, FormatConditionValueType.Percent);
[Test]
        public void Type_FormatConditionValueType()
        {
            String sfilePath = Constants.sourcePath + "ConditionalFormattings\\TestIconSetCopy.xlsx";
            String dfilePath = Constants.destPath + "TestIconSetCopy.xlsx";

            Workbook book = new Workbook(sfilePath);
            ConditionalFormattingCollection cfs = book.Worksheets[0].ConditionalFormattings;
            book.Worksheets[1].ConditionalFormattings.Copy(cfs);
            book.Save(dfilePath);
            Workbook newbook = new Workbook(dfilePath);
            ConditionalFormattingCollection newcfs = newbook.Worksheets[1].ConditionalFormattings;
            FormatConditionCollection fcs = newcfs[0];
            FormatCondition fc = fcs[0];

            FormatConditionType type = fc.Type;
            int priority = fc.Priority;
            IconSetType iconSet = fc.IconSet.Type;
            FormatConditionValueType valueType = fc.IconSet.Cfvos[0].Type;
            object value = fc.IconSet.Cfvos[0].Value;
            FormatConditionValueType valueType1 = fc.IconSet.Cfvos[1].Type;
            object value1 = fc.IconSet.Cfvos[1].Value;
            FormatConditionValueType valueType2 = fc.IconSet.Cfvos[2].Type;
            object value2 = fc.IconSet.Cfvos[2].Value;

            ConditionalFormattingIcon cficon = fc.IconSet.CfIcons[0];
            IconSetType cficonType = cficon.Type;
            int cficonId = cficon.Index;
            ConditionalFormattingIcon cficon1 = fc.IconSet.CfIcons[1];
            IconSetType cficon1Type = cficon1.Type;
            int cficonId1 = cficon1.Index;
            ConditionalFormattingIcon cficon2 = fc.IconSet.CfIcons[2];
            IconSetType cficon2Type = cficon2.Type;
            int cficonId2 = cficon2.Index;

            string sqref = GetCellAreaName(fcs.GetCellArea(0));

            Assert.AreEqual(type, FormatConditionType.IconSet);
            Assert.AreEqual(priority, 1);
            Assert.AreEqual(iconSet, IconSetType.CustomSet);
            Assert.AreEqual(valueType, FormatConditionValueType.Percent);
            Assert.AreEqual((int)value, 0);
            Assert.AreEqual(valueType1, FormatConditionValueType.Percent);
            Assert.AreEqual((int)value1, 33);
            Assert.AreEqual(valueType2, FormatConditionValueType.Percent);
            Assert.AreEqual((int)value2, 67);

            Assert.AreEqual(cficonType, IconSetType.Flags3);
            Assert.AreEqual(cficonId, 2);
            Assert.AreEqual(cficon1Type, IconSetType.TrafficLights31);
            Assert.AreEqual(cficonId1, 0);
            Assert.AreEqual(cficon2Type, IconSetType.Arrows3);
            Assert.AreEqual(cficonId2, 0);

            Assert.AreEqual(sqref, "A1:C1");
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


