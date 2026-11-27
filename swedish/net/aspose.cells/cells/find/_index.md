---
title: "Cells.Find"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells‑metod. Hittar cellen som innehåller det angivna objektet"
type: docs
url: /sv/net/aspose.cells/cells/find/
---
## Find(object, Cell) {#find}

Hittar cellen som innehåller det angivna objektet.

```csharp
public Cell Find(object what, Cell previousCell)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| vad | Object | Objektet att söka efter. Typen bör vara int,double,DateTime,string,bool. |
| previousCell | Cell | Föregående cell med samma objekt. Denna parameter kan sättas till null om sökningen startas från början. |

### Returvärde

Cellobjekt.

### Anmärkningar

Returnerar null (Nothing) om ingen cell hittas.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodFindWithObjectCellDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1.2);

            // Hitta cellen som innehåller "Orange"
            Cell searchCell = null;
            Cell foundCell = worksheet.Cells.Find("Orange", searchCell);

            if (foundCell != null)
            {
                Console.WriteLine("Found 'Orange' at: " + foundCell.Name);
                
                // Skapa och tillämpa en stil på den hittade cellen
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Red;
                style.Font.IsBold = true;
                foundCell.SetStyle(style);
            }

            // Spara arbetsboken
            workbook.Save("FindMethodDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Find(object, Cell, FindOptions) {#find_1}

Hittar cellen som innehåller det angivna objektet.

```csharp
public Cell Find(object what, Cell previousCell, FindOptions findOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| vad | Object | Objektet att söka efter. Typen bör vara int,double,DateTime,string,bool. |
| previousCell | Cell | Föregående cell med samma objekt. Denna parameter kan sättas till null om sökningen startas från början. |
| findOptions | FindOptions | Sökalternativ |

### Returvärde

Cellobjekt.

### Anmärkningar

Returnerar null (Nothing) om ingen cell hittas.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodFindWithObjectCellFindOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange exempeldata
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["A2"].PutValue("def");
            worksheet.Cells["A3"].PutValue("abc ");
            
            // Skapa sökalternativ
            FindOptions options = new FindOptions();
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;
            
            // Hitta cell med värdet "abc "
            Cell foundCell = worksheet.Cells.Find("abc ", null, options);
            
            Console.WriteLine("Found cell: " + (foundCell != null ? foundCell.Name : "null"));
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [FindOptions](../../findoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


