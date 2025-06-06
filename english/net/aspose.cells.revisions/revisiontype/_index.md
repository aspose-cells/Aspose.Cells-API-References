---
title: Enum RevisionType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.RevisionType enum. Represents the revision type
type: docs
url: /net/aspose.cells.revisions/revisiontype/
---
## RevisionType enumeration

Represents the revision type.

```csharp
public enum RevisionType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| CustomView | `0` | Custom view. |
| DefinedName | `1` | Defined name. |
| ChangeCells | `2` | Cells change. |
| AutoFormat | `3` | Auto format. |
| MergeConflict | `4` | Merge conflict. |
| Comment | `5` | Comment. |
| Format | `6` | Format. |
| InsertSheet | `7` | Insert worksheet. |
| MoveCells | `8` | Move cells. |
| Undo | `9` | Undo. |
| QueryTable | `10` | Query table. |
| InsertDelete | `11` | Inserting or deleting. |
| RenameSheet | `12` | Rename worksheet. |
| Unknown | `13` | Unknown. |

### Examples

```csharp
// Called: case RevisionType.Format:
private void Revisions_Type_RevisionType(string file)
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

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


