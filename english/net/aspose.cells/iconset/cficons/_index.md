---
title: IconSet.CfIcons
second_title: Aspose.Cells for .NET API Reference
description: IconSet property. Get theConditionalFormattingIcon from the collection
type: docs
url: /net/aspose.cells/iconset/cficons/
---
## IconSet.CfIcons property

Get the[`ConditionalFormattingIcon`](../../conditionalformattingicon/) from the collection

```csharp
public ConditionalFormattingIconCollection CfIcons { get; }
```

### Examples

```csharp
// Called: ConditionalFormattingIconCollection iconCollection = condition.IconSet.CfIcons;
[Test]
        public void Property_CfIcons()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "ConditionalFormattings/CELLSJAVA42328.xlsm");
            Worksheet sheet1 = workbook.Worksheets[1];

            ConditionalFormattingCollection collection = sheet1.ConditionalFormattings;
            //  for(int i = 0; i < collection.Count; i++)
            {
                int i = 2;
                FormatConditionCollection conditionCollection = collection[i];

            //    for (int j = 0; j < conditionCollection.Count; j++)
                {
                    FormatCondition condition = conditionCollection[0];
                    //if(condition.getType() == FormatConditionType.ICON_SET){ 
                    ConditionalFormattingIconCollection iconCollection = condition.IconSet.CfIcons;

                    Assert.AreEqual(2, iconCollection[0].Index);
                    Assert.AreEqual(2, iconCollection[1].Index);
                    Assert.AreEqual(0, iconCollection[2].Index);
                }
            } 
        }
```

### See Also

* class [ConditionalFormattingIconCollection](../../conditionalformattingiconcollection/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


