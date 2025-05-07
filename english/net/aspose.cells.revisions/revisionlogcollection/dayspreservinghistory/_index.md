---
title: RevisionLogCollection.DaysPreservingHistory
second_title: Aspose.Cells for .NET API Reference
description: RevisionLogCollection property. Gets and sets the number of days the spreadsheet application will keep the change history for this workbook
type: docs
url: /net/aspose.cells.revisions/revisionlogcollection/dayspreservinghistory/
---
## RevisionLogCollection.DaysPreservingHistory property

Gets and sets the number of days the spreadsheet application will keep the change history for this workbook.

```csharp
public int DaysPreservingHistory { get; set; }
```

### Examples

```csharp
// Called: workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 40;
[Test]
        public void Property_DaysPreservingHistory()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Worksheets[0].Cells["A1"].PutValue("sdfsdf");
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 40;
            workbook.Save(Constants.destPath + "CellsNet45791.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet45791.xlsx");
            Assert.AreEqual(40, workbook.Worksheets.RevisionLogs.DaysPreservingHistory);
            workbook.Save(Constants.destPath + "CellsNet45791.xlsx");

        }
```

### See Also

* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


