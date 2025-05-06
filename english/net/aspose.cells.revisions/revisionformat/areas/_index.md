---
title: RevisionFormat.Areas
second_title: Aspose.Cells for .NET API Reference
description: RevisionFormat property. The range to which this formatting was applied
type: docs
url: /net/aspose.cells.revisions/revisionformat/areas/
---
## RevisionFormat.Areas property

The range to which this formatting was applied.

```csharp
public CellArea[] Areas { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(string.Format(&amp;quot;worksheet :{0}; area : {1}.&amp;quot;, rfmt.Worksheet.Name, rfmt.Areas[0]));
private void Property_Areas(string file)
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


