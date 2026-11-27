---
title: "ListObject.ListColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject-egenskap. Hämtar ListColumn-listan för den här tabellen"
type: docs
url: /sv/net/aspose.cells.tables/listobject/listcolumns/
---
## ListObject.ListColumns property

Hämtar [`ListColumn`](../../listcolumn/)-listan för den här tabellen.

```csharp
public ListColumnCollection ListColumns { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyListColumnsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
                }
            }

            // Skapa ett listobjekt
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add(0, 0, 9, 4, true);
            ListObject listObject = listObjects[index];
            
            // Aktivera totaler och ange beräkning för den 5:e kolumnen
            listObject.ShowTotals = true;
            listObject.ListColumns[4].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
            
            // Använd tabellstil
            listObject.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleLight4;

            // Spara arbetsboken
            workbook.Save("ListColumnsDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [ListColumnCollection](../../listcolumncollection/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


