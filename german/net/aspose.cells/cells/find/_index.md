---
title: "Cells.Find"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Findet die Zelle, die das Eingabeobjekt enthält"
type: docs
url: /de/net/aspose.cells/cells/find/
---
## Find(object, Cell) {#find}

Findet die Zelle, die das Eingabeobjekt enthält.

```csharp
public Cell Find(object what, Cell previousCell)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| was | Object | Das zu suchende Objekt. Der Typ sollte int,double,DateTime,string,bool sein. |
| previousCell | Zelle | Vorherige Zelle mit demselben Objekt. Dieser Parameter kann auf null gesetzt werden, wenn von Anfang an gesucht wird. |

### Rückgabewert

Zellobjekt.

### Hinweise

Gibt null (Nothing) zurück, wenn keine Zelle gefunden wird.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodFindWithObjectCellDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1.2);

            // Finde die Zelle, die "Orange" enthält
            Cell searchCell = null;
            Cell foundCell = worksheet.Cells.Find("Orange", searchCell);

            if (foundCell != null)
            {
                Console.WriteLine("Found 'Orange' at: " + foundCell.Name);
                
                // Erstelle und wende einen Stil auf die gefundene Zelle an
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Red;
                style.Font.IsBold = true;
                foundCell.SetStyle(style);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("FindMethodDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Find(object, Cell, FindOptions) {#find_1}

Findet die Zelle, die das Eingabeobjekt enthält.

```csharp
public Cell Find(object what, Cell previousCell, FindOptions findOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| was | Object | Das zu suchende Objekt. Der Typ sollte int,double,DateTime,string,bool sein. |
| previousCell | Zelle | Vorherige Zelle mit demselben Objekt. Dieser Parameter kann auf null gesetzt werden, wenn von Anfang an gesucht wird. |
| findOptions | FindOptions | Suchoptionen |

### Rückgabewert

Zellobjekt.

### Hinweise

Gibt null (Nothing) zurück, wenn keine Zelle gefunden wird.

### Beispiele

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
            
            // Beispieldaten festlegen
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["A2"].PutValue("def");
            worksheet.Cells["A3"].PutValue("abc ");
            
            // Suchoptionen erstellen
            FindOptions options = new FindOptions();
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;
            
            // Finde Zelle mit dem Wert "abc "
            Cell foundCell = worksheet.Cells.Find("abc ", null, options);
            
            Console.WriteLine("Found cell: " + (foundCell != null ? foundCell.Name : "null"));
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [FindOptions](../../findoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


