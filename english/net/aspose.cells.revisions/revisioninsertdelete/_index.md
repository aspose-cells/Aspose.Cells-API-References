---
title: Class RevisionInsertDelete
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.RevisionInsertDelete class. Represents a revision record of a row/column insert/delete action
type: docs
url: /net/aspose.cells.revisions/revisioninsertdelete/
---
## RevisionInsertDelete class

Represents a revision record of a row/column insert/delete action.

```csharp
public class RevisionInsertDelete : Revision
```

## Properties

| Name | Description |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertdelete/actiontype/) { get; } | Gets the action type of this revision. |
| [CellArea](../../aspose.cells.revisions/revisioninsertdelete/cellarea/) { get; } | Gets the inserting/deleting range. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Gets the number of this revision.(Inherited from [`Revision`](../revision/).) |
| [Revisions](../../aspose.cells.revisions/revisioninsertdelete/revisions/) { get; } | Gets revision list by this operation. |
| override [Type](../../aspose.cells.revisions/revisioninsertdelete/type/) { get; } | Represents the type of revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Gets the worksheet.(Inherited from [`Revision`](../revision/).) |

### Examples

```csharp
// Called: RevisionInsertDelete rrc = (RevisionInsertDelete)rv;
private void Type_RevisionInsertDelete(string file)
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
                            Console.WriteLine(string.Format(&quot;ActionType :{0}; newArea : {1}.&quot;, rrc.ActionType, rrc.CellArea));
                            Console.WriteLine(rrc.CellArea);
                            break;
                        case RevisionType.ChangeCells:
                            RevisionCellChange rcc = (RevisionCellChange)rv;
                            string str = string.Format(&quot;CellName :{0}; OldValue : {1} ;NewOld : {2}.&quot;, rcc.CellName, rcc.OldValue, rcc.NewValue);
                            Console.WriteLine(str);
                            break;
                        case RevisionType.MoveCells:
                            RevisionCellMove rm = (RevisionCellMove)rv;
                            Console.WriteLine(string.Format(&quot;SourceArea :{0}; newArea : {1}.&quot;, rm.SourceArea, rm.DestinationArea));
                            break;
                        case RevisionType.CustomView:
                            RevisionCustomView rcv = (RevisionCustomView)rv;
                            Console.WriteLine(string.Format(&quot;ActionType :{0}; guid : {1}.&quot;, rcv.ActionType, rcv.Guid));
                            break;
                        case RevisionType.Format:
                            RevisionFormat rfmt = (RevisionFormat)rv;
                            Console.WriteLine(string.Format(&quot;worksheet :{0}; area : {1}.&quot;, rfmt.Worksheet.Name, rfmt.Areas[0]));
                            break;
                        case RevisionType.InsertSheet:
                            RevisionInsertSheet ris = (RevisionInsertSheet)rv;
                            Console.WriteLine(string.Format(&quot;newsheet :{0}; sheetPosition : {1}.&quot;, ris.Name, ris.SheetPosition));
                            break;
                        case RevisionType.DefinedName:
                            RevisionDefinedName rdn = (RevisionDefinedName)rv;
                            Console.WriteLine(string.Format(&quot;Test :{0}; oldFormula :{1};  newformula : {2}.&quot;, rdn.Text, rdn.OldFormula, rdn.NewFormula));

                            break;
                        case RevisionType.RenameSheet:
                            RevisionRenameSheet rsnm = (RevisionRenameSheet)rv;
                            Console.WriteLine(string.Format(&quot;OldName :{0}; newName :{1}.&quot;, rsnm.OldName, rsnm.NewName));
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


