---
title: ConditionalFormattingIcon.Index
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingIcon property. Gets and sets the icons index in the icon set
type: docs
url: /net/aspose.cells/conditionalformattingicon/index/
---
## ConditionalFormattingIcon.Index property

Gets and sets the icon's index in the icon set.

```csharp
public int Index { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(0, iconCollection[2].Index);
[Test]
        public void Property_Index()
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

* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


