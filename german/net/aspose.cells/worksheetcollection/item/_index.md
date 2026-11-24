---
title: "WorksheetCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Eigenschaft. Gibt das Worksheet-Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/worksheetcollection/item/
---
## WorksheetCollection indexer (1 of 2)

Gibt das [`Worksheet`](../../worksheet/) Element am angegebenen Index zurück.

```csharp
public Worksheet this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Verwenden der Item-Eigenschaft zum Zugriff auf Zelle
            Cell cell = cells[0, 0];
            cell.Formula = "=SUM(1, 2, 3)";
            
            workbook.CalculateFormula();
            Console.WriteLine("Cell value: " + cell.IntValue);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorksheetCollection indexer (2 of 2)

Gibt das [`Worksheet`](../../worksheet/) Element mit dem angegebenen Namen zurück.

```csharp
public Worksheet this[string sheetName] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| sheetName | Arbeitsblattname |

### Rückgabewert

Das Element mit dem angegebenen Namen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf Arbeitsblätter mittels Item-Eigenschaft nach Index und Name
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            
            // Zugriff auf das Arbeitsblatt nach Namen über die Item-Eigenschaft
            Worksheet accessedSheet = workbook.Worksheets["FirstSheet"];
            
            // Füge Daten hinzu, um den Zugriff auf das Arbeitsblatt zu demonstrieren
            Cells cells = accessedSheet.Cells;
            cells["A1"].PutValue("Worksheet accessed successfully!");
            cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Füge eine Spalte im zweiten Blatt ein
            workbook.Worksheets["SecondSheet"].Cells.InsertColumn(1);
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetCollectionItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


