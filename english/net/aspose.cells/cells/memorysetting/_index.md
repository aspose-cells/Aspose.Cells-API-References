---
title: Cells.MemorySetting
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets or sets the memory usage option for this cells
type: docs
url: /net/aspose.cells/cells/memorysetting/
---
## Cells.MemorySetting property

Gets or sets the memory usage option for this cells.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Examples

```csharp
// Called: cells.MemorySetting = MemorySetting.MemoryPreference;
[Test]
        public void Property_MemorySetting()
        {
            //LoadOptions opts = new LoadOptions(LoadFormat.Xlsx);
            //opts.MemorySetting = MemorySetting.MemoryPreference;
            //Workbook wb1 = new Workbook(Constants.sourcePath + &quot;Cells/41596_671930.xlsx&quot;, opts); //loading with memory mode will not cause the issue
            Workbook wb = new Workbook(Constants.sourcePath + &quot;Cells/J41596_671930.xlsx&quot;);//, opts);
            wb.Settings.MemorySetting = MemorySetting.MemoryPreference;
            Worksheet sheet = wb.Worksheets[&quot;Data&quot;];
            Cells cells = sheet.Cells;
            cells.MemorySetting = MemorySetting.MemoryPreference;
            string[] rns = new string[]{
                &quot;R_externalIncoming&quot;, &quot;R_degradedExternalIncoming&quot;, &quot;R_failedExternalIncoming&quot;, &quot;R_toPSTNs&quot;, &quot;R_degradedToPSTNs&quot;,
                &quot;R_failedToPSTNs&quot;, &quot;R_degradedCauseNoCLIHidden&quot;, &quot;R_degradedCauseNoRouteToTerminal&quot;, &quot;R_failedCauseNoRouteToTerminal&quot;,

            };
            //CellsException: Cell has been removed: R108
            foreach (string rn in rns)
            {
                Aspose.Cells.Range anyRange = wb.Worksheets.GetRangeByName(rn);
                int firstRowIndex = anyRange.FirstRow;
                cells.InsertRows(firstRowIndex + 1, 16);
                ArrayList list = new ArrayList();
                Row row = cells.Rows[firstRowIndex + 17];
                IEnumerator en = row.GetEnumerator();
                while (en.MoveNext())
                {
                    list.Add(en.Current);
                }
                Cell[] srcs = new Cell[list.Count];
                for(int i=0; i&lt;srcs.Length; i++)
                {
                    srcs[i] = (Cell)list[i];
                }
                en = null;
                row = null;
                list = null;
                for (int i = 0; i &lt; 8; i++)
                {
                    cells.CopyRow(cells, firstRowIndex + 17, firstRowIndex + 1 + 2 * i); // even rows
                    Row rowDest = cells.Rows[firstRowIndex + 1 + 2 * i];
                    for (int j = 0; j &lt; srcs.Length; j++)
                    {
                        Cell sc = srcs[j];
                        if (sc.IsFormula)
                        {
                            Assert.IsTrue(rowDest[sc.Column].IsFormula, rn + &quot;-&quot; + i + &quot;-&quot; + j);
                        }
                        else
                        {
                            WorkbookCompare.CellTest.equalsValue(sc, rowDest[sc.Column], rn + &quot;-&quot; + i + &quot;-&quot; + j);
                        }
                    }
                }
                for (int i = 0; i &lt; 8; i++)
                {
                    cells.CopyRow(cells, firstRowIndex, firstRowIndex + 2 + 2 * i); // odd rows
                }
            }
        }
```

### See Also

* enum [MemorySetting](../../memorysetting/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


