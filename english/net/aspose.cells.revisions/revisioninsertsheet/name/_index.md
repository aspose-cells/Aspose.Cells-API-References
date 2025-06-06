---
title: RevisionInsertSheet.Name
second_title: Aspose.Cells for .NET API Reference
description: RevisionInsertSheet property. Gets the name of the worksheet
type: docs
url: /net/aspose.cells.revisions/revisioninsertsheet/name/
---
## RevisionInsertSheet.Name property

Gets the name of the worksheet.

```csharp
public string Name { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(string.Format("newsheet :{0}; sheetPosition : {1}.", ris.Name, ris.SheetPosition));
private void RevisionInsertSheet_Property_Name(string file)
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

* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


