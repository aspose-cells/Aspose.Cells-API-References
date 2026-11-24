---
title: "ListColumnCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListColumnCollection‑Eigenschaft. Gibt das ListColumn nach dem Index zurück"
type: docs
url: /de/net/aspose.cells.tables/listcolumncollection/item/
---
## ListColumnCollection indexer (1 of 2)

Gibt das ListColumn anhand des Index zurück.

```csharp
public ListColumn this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Rückgabewert

das ListColumn‑Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("T1");
            worksheet.Cells["B1"].PutValue("T2");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);

            // Erstelle ein Listenobjekt
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObj = worksheet.ListObjects[index];
            
            // Greife auf Listenspalten zu, indem du die Item‑Eigenschaft verwendest
            ListColumn firstColumn = listObj.ListColumns[0];
            Console.WriteLine("First column name: " + firstColumn.Name);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ListColumnCollection indexer (2 of 2)

Gibt das ListColumn anhand des Namens zurück.

```csharp
public ListColumn this[string name] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Name | Der Name des ListColumn |

### Rückgabewert

Das ListColumn‑Objekt.

### Siehe auch

* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


