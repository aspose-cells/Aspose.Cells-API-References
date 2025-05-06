---
title: RevisionLog.Revisions
second_title: Aspose.Cells for .NET API Reference
description: RevisionLog property. Gets all revisions in this log
type: docs
url: /net/aspose.cells.revisions/revisionlog/revisions/
---
## RevisionLog.Revisions property

Gets all revisions in this log.

```csharp
public RevisionCollection Revisions { get; }
```

### Examples

```csharp
// Called: RevisionCollection rvs = log.Revisions;
[Test]
        public void Property_Revisions()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;Revision/N50333.xlsx&quot;);
            Assert.IsTrue(wb.HasRevisions, &quot;Workbook.HasRevision&quot;);
            RevisionLogCollection rlc = wb.Worksheets.RevisionLogs;
            Assert.AreEqual(3, rlc.Count, &quot;Revision logs count&quot;);
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
                                Assert.AreEqual(&quot;Sheet2!A1&quot;, fml, rcc.CellName);
                                matched++;
                            }
                            else if (rcc.Row == 1)
                            {
                                Assert.AreEqual(&quot;Sheet2!#REF!&quot;, fml, rcc.CellName);
                                matched++;
                            }
                        }
                    }
                }
            }
            Assert.AreEqual(2, matched, &quot;Changed formula count&quot;);
        }
```

### See Also

* class [RevisionCollection](../../revisioncollection/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


