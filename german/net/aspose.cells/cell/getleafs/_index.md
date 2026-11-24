---
title: "Cell.GetLeafs"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt alle Zellen zurück, die direkt auf diese Zelle verweisen und aktualisiert werden müssen, wenn diese Zelle geändert wird"
type: docs
url: /de/net/aspose.cells/cell/getleafs/
---
## GetLeafs() {#getleafs}

Alle Zellen abrufen, die direkt auf diese Zelle verweisen und aktualisiert werden müssen, wenn diese Zelle geändert wird.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs()
```

### Rückgabewert

Enumerator zum Auflisten aller abhängigen Zellen (Cell)

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Bitte verwenden Sie stattdessen Cell.GetDependentsInCalculation(bool), um alle abhängigen Elemente in der Berechnungskette zu erhalten. Diese Eigenschaft wird 12 Monate nach Mai 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Daten und Formeln hinzufügen, um Abhängigkeiten zu erstellen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Hole die Zelle, die abhängige Zellen hat
                Cell cell = worksheet.Cells["B1"];

                // Rufen Sie GetLeafs auf, um alle Zellen zu erhalten, die diese Zelle direkt referenzieren
                IEnumerator leafs = cell.GetLeafs();

                Console.WriteLine("Cells that directly reference B1:");
                while (leafs.MoveNext())
                {
                    Cell leafCell = leafs.Current as Cell;
                    if (leafCell != null)
                    {
                        Console.WriteLine($"Cell: {leafCell.Name}, Formula: {leafCell.Formula}");
                    }
                }

                // Speichere die Arbeitsmappe
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetLeafs(bool) {#getleafs_1}

Alle Zellen abrufen, die aktualisiert werden, wenn diese Zelle geändert wird.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs(bool recursive)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rekursiv | Boolean | Ob diejenigen Blätter zurückgegeben werden, die nicht direkt auf diese Zelle verweisen, sondern auf andere Blätter dieser Zelle |

### Rückgabewert

Enumerator zum Auflisten aller abhängigen Zellen (Cell)

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Bitte verwenden Sie stattdessen Cell.GetDependentsInCalculation(bool), um alle abhängigen Elemente in der Berechnungskette zu erhalten. Diese Eigenschaft wird 12 Monate nach Mai 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Daten mit Formeln hinzu, um Abhängigkeiten zu erstellen
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Hole die Zelle, die abhängige Zellen hat
                Cell cell = worksheet.Cells["A1"];

                // Rufen Sie GetLeafs mit dem rekursiven Parameter auf, der auf true gesetzt ist
                IEnumerator leafs = cell.GetLeafs(true);

                // Ergebnisse anzeigen
                Console.WriteLine("Leaf cells found:");
                while (leafs.MoveNext())
                {
                    Cell leaf = (Cell)leafs.Current;
                    Console.WriteLine($"Cell: {leaf.Name}, Value: {leaf.Value}");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


