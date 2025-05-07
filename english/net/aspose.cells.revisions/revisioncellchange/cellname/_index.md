---
title: RevisionCellChange.CellName
second_title: Aspose.Cells for .NET API Reference
description: RevisionCellChange property. Gets the name of the cell
type: docs
url: /net/aspose.cells.revisions/revisioncellchange/cellname/
---
## RevisionCellChange.CellName property

Gets the name of the cell.

```csharp
public string CellName { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("Sheet2!#REF!", fml, rcc.CellName);
[Test]
        public void Property_CellName()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "Revision/N50333.xlsx");
            Assert.IsTrue(wb.HasRevisions, "Workbook.HasRevision");
            RevisionLogCollection rlc = wb.Worksheets.RevisionLogs;
            Assert.AreEqual(3, rlc.Count, "Revision logs count");
            int matched = 0;
            foreach (RevisionLog log in rlc)
            {
                RevisionCollection rvs = log.Revisions;
                foreach (Revision rv in rvs)
                {
                    if (rv.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange rcc = (RevisionCellChange)rv;
                        string fml = rcc.OldFormula;
                        if (fml != null)
                        {
                            if (rcc.Row == 0)
                            {
                                Assert.AreEqual("Sheet2!A1", fml, rcc.CellName);
                                matched++;
                            }
                            else if (rcc.Row == 1)
                            {
                                Assert.AreEqual("Sheet2!#REF!", fml, rcc.CellName);
                                matched++;
                            }
                        }
                    }
                }
            }
            Assert.AreEqual(2, matched, "Changed formula count");
        }
```

### See Also

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


