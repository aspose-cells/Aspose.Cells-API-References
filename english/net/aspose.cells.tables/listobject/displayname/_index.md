---
title: ListObject.DisplayName
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets the display name
type: docs
url: /net/aspose.cells.tables/listobject/displayname/
---
## ListObject.DisplayName property

Gets and sets the display name.

```csharp
public string DisplayName { get; set; }
```

### Examples

```csharp
// Called: string tname = ws.ListObjects[i].DisplayName;
[Test]
        public void Property_DisplayName()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet46085.xlsx");
            Worksheet ws = workbook.Worksheets["Pg2 Acct Code Breakdown"];

            ArrayList dNames = new ArrayList();
            for (int i = 0; i < ws.ListObjects.Count; i++)
            {
                string tname = ws.ListObjects[i].DisplayName;
                dNames.Add(tname);

            }

            if (dNames.Count != 0)
            {
                for (int i = 0; i < dNames.Count; i++)
                {
                    string tname = dNames[i].ToString();
                    ListObject listObject = ws.ListObjects[tname];
                    listObject.ConvertToRange();//Exception
                }
            }

            workbook.Save(Constants.destPath + "CellsNet46085.xlsx");
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


