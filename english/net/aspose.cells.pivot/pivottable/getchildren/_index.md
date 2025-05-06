---
title: PivotTable.GetChildren
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Gets the Children Pivot Tables which use this PivotTable data as data source
type: docs
url: /net/aspose.cells.pivot/pivottable/getchildren/
---
## PivotTable.GetChildren method

Gets the Children Pivot Tables which use this PivotTable data as data source.

```csharp
public PivotTable[] GetChildren()
```

### Return Value

the PivotTable array object

### Examples

```csharp
// Called: int childrenLen = table.GetChildren().Length;
[Test]
        public void Method_GetChildren()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET46707_&quot;;

            using (Workbook workbook = new Workbook(filePath + &quot;AsposeIn.xlsx&quot;))
            {
                foreach (Worksheet worksheet in workbook.Worksheets)
                {
                    worksheet.RefreshPivotTables();
                    foreach (PivotTable table in worksheet.PivotTables)
                    {
                        //childrenCounts.Add(worksheet.Name, table.GetChildren().Length);
                        int childrenLen = table.GetChildren().Length;
                        switch (worksheet.Name)
                        {
                            case &quot;Calculs1&quot;:
                                Assert.AreEqual(childrenLen, 0);
                                break;
                            case &quot;Calculs2&quot;:
                            case &quot;Calculs3&quot;:
                            case &quot;Calculs4&quot;:
                                Assert.AreEqual(childrenLen, 1);
                                break;
                            default:
                                break;
                        }

                        Console.WriteLine(string.Format(&quot;{0},{1}&quot;, worksheet.Name, childrenLen));
                    }
                }
            }
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


