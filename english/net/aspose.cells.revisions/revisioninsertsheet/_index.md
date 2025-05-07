---
title: Class RevisionInsertSheet
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.RevisionInsertSheet class. Represents a revision record of a sheet that was inserted
type: docs
url: /net/aspose.cells.revisions/revisioninsertsheet/
---
## RevisionInsertSheet class

Represents a revision record of a sheet that was inserted.

```csharp
public class RevisionInsertSheet : Revision
```

## Properties

| Name | Description |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertsheet/actiontype/) { get; } | Gets the action type of the revision. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Gets the number of this revision.(Inherited from [`Revision`](../revision/).) |
| [Name](../../aspose.cells.revisions/revisioninsertsheet/name/) { get; } | Gets the name of the worksheet. |
| [SheetPosition](../../aspose.cells.revisions/revisioninsertsheet/sheetposition/) { get; } | Gets the zero based position of the new sheet in the sheet tab bar. |
| override [Type](../../aspose.cells.revisions/revisioninsertsheet/type/) { get; } | Gets the type of revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Gets the worksheet.(Inherited from [`Revision`](../revision/).) |

### Examples

```csharp
// Called: RevisionInsertSheet ris = (RevisionInsertSheet)rv;
private void Type_RevisionInsertSheet(string file)
        {
            Workbook workbook = new Workbook(file);
            foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
            {
                RevisionCollection rvs = log.Revisions;
                foreach (Revision rv in rvs)
                {
                    switch (rv.Type)
                    {

                        case RevisionType.InsertDelete:
                            RevisionInsertDelete rrc = (RevisionInsertDelete)rv;
                            Console.WriteLine(string.Format("ActionType :{0}; newArea : {1}.", rrc.ActionType, rrc.CellArea));
                            Console.WriteLine(rrc.CellArea);
                            break;
                        case RevisionType.ChangeCells:
                            RevisionCellChange rcc = (RevisionCellChange)rv;
                            string str = string.Format("CellName :{0}; OldValue : {1} ;NewOld : {2}.", rcc.CellName, rcc.OldValue, rcc.NewValue);
                            Console.WriteLine(str);
                            break;
                        case RevisionType.MoveCells:
                            RevisionCellMove rm = (RevisionCellMove)rv;
                            Console.WriteLine(string.Format("SourceArea :{0}; newArea : {1}.", rm.SourceArea, rm.DestinationArea));
                            break;
                        case RevisionType.CustomView:
                            RevisionCustomView rcv = (RevisionCustomView)rv;
                            Console.WriteLine(string.Format("ActionType :{0}; guid : {1}.", rcv.ActionType, rcv.Guid));
                            break;
                        case RevisionType.Format:
                            RevisionFormat rfmt = (RevisionFormat)rv;
                            Console.WriteLine(string.Format("worksheet :{0}; area : {1}.", rfmt.Worksheet.Name, rfmt.Areas[0]));
                            break;
                        case RevisionType.InsertSheet:
                            RevisionInsertSheet ris = (RevisionInsertSheet)rv;
                            Console.WriteLine(string.Format("newsheet :{0}; sheetPosition : {1}.", ris.Name, ris.SheetPosition));
                            break;
                        case RevisionType.DefinedName:
                            RevisionDefinedName rdn = (RevisionDefinedName)rv;
                            Console.WriteLine(string.Format("Test :{0}; oldFormula :{1};  newformula : {2}.", rdn.Text, rdn.OldFormula, rdn.NewFormula));

                            break;
                        case RevisionType.RenameSheet:
                            RevisionRenameSheet rsnm = (RevisionRenameSheet)rv;
                            Console.WriteLine(string.Format("OldName :{0}; newName :{1}.", rsnm.OldName, rsnm.NewName));
                            break;
                        default:
                            Console.WriteLine(rv.Type);
                            break;
                    }
                }
            }
        }
```

### See Also

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


