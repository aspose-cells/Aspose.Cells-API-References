---
title: ConditionalFormattingIconCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingIconCollection property. Gets the ConditionalFormattingIcon element at the specified index
type: docs
url: /net/aspose.cells/conditionalformattingiconcollection/item/
---
## ConditionalFormattingIconCollection indexer

Gets the ConditionalFormattingIcon element at the specified index.

```csharp
public ConditionalFormattingIcon this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: ConditionalFormattingIcon cficon = fc.IconSet.CfIcons[0];
[Test]
        public void Property_Int32_()
        {
            String sfilePath = Constants.sourcePath + &quot;ConditionalFormattings\\TestIconSetCopy.xlsx&quot;;
            String dfilePath = Constants.destPath + &quot;TestIconSetCopy.xlsx&quot;;

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

            Assert.AreEqual(sqref, &quot;A1:C1&quot;);
        }
```

### See Also

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


