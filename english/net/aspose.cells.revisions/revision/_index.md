---
title: Class Revision
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.Revision class. Represents the revision
type: docs
url: /net/aspose.cells.revisions/revision/
---
## Revision class

Represents the revision.

```csharp
public abstract class Revision
```

## Properties

| Name | Description |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Gets the number of this revision. |
| virtual [Type](../../aspose.cells.revisions/revision/type/) { get; } | Represents the type of revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Gets the worksheet. |

### Examples

```csharp
// Called: foreach (Revision rv in rvs)
[Test]
        public void Type_Revision()
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

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


