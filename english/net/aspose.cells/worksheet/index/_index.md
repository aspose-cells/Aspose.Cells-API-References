---
title: Worksheet.Index
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the index of sheet in the worksheet collection
type: docs
url: /net/aspose.cells/worksheet/index/
---
## Worksheet.Index property

Gets the index of sheet in the worksheet collection.

```csharp
public int Index { get; }
```

### Examples

```csharp
// Called: mFormatCondition = sheet.Index + "-" + i + "-" + j;
public override void Worksheet_Property_Index(FormatCondition fc)
            {
                bool found = false;
                foreach (Worksheet sheet in mWorkbook.Worksheets)
                {
                    for (int i = sheet.ConditionalFormattings.Count - 1; i > -1; i--)
                    {
                        FormatConditionCollection fcc = sheet.ConditionalFormattings[i];
                        for (int j = fcc.Count - 1; j > -1; j--)
                        {
                            if (fc == fcc[j])
                            {
                                mFormatCondition = sheet.Index + "-" + i + "-" + j;
                                found = true;
                                break;
                            }
                        }
                        if (found)
                        {
                            break;
                        }

                    }
                    if (found)
                    {
                        break;
                    }
                }
            }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


