---
title: Revision.Type
second_title: Aspose.Cells for .NET API Reference
description: Revision property. Represents the type of revision
type: docs
url: /net/aspose.cells.revisions/revision/type/
---
## Revision.Type property

Represents the type of revision.

```csharp
public virtual RevisionType Type { get; }
```

### Examples

```csharp
// Called: if (rv.Type == RevisionType.ChangeCells)
public void Revision_Property_Type()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
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

* enum [RevisionType](../../revisiontype/)
* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


