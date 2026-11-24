---
title: "AutoFilter.GetCellArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Methode. Gibt den CellArea zurück, auf den dieser AutoFilter angewendet wird"
type: docs
url: /de/net/aspose.cells/autofilter/getcellarea/
---
## GetCellArea() {#getcellarea}

Gibt den [`CellArea`](../../cellarea/) zurück, auf den dieser AutoFilter angewendet wird.

```csharp
public CellArea GetCellArea()
```

### Rückgabewert

der Bereich, auf den dieser Filter angewendet wird

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispieldaten für die AutoFilter-Demonstration füllen
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Category");
            cells["C1"].PutValue("Price");

            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue("Fruit");
            cells["C2"].PutValue(2.5);

            cells["A3"].PutValue("Carrot");
            cells["B3"].PutValue("Vegetable");
            cells["C3"].PutValue(1.2);

            cells["A4"].PutValue("Banana");
            cells["B4"].PutValue("Fruit");
            cells["C4"].PutValue(3.1);

            // AutoFilter auf Kopfzeilen (Zeilenindex 0) anwenden, die die Spalten A-C (0-2) abdecken
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.SetRange(0, 0, 2);

            try
            {
                // Den CellArea abrufen, auf den AutoFilter angewendet wird
                CellArea result = autoFilter.GetCellArea();

                // Die Koordinaten des AutoFilter-Bereichs ausgeben
                Console.WriteLine("AutoFilter applied to cell area:");
                Console.WriteLine($"Start Row: {result.StartRow}");
                Console.WriteLine($"Start Column: {result.StartColumn}");
                Console.WriteLine($"End Row: {result.EndRow}");
                Console.WriteLine($"End Column: {result.EndColumn}");

                // Einen einfachen Filter anwenden, um die Funktionalität zu demonstrieren (optional)
                autoFilter.Filter(1, "Fruit"); // Filter "Category" column (index 1) for "Fruit"
                autoFilter.Refresh();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea method: {ex.Message}");
            }

            // Die Arbeitsmappe mit angewendetem AutoFilter speichern
            workbook.Save("AutoFilterMethodGetCellAreaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellArea(bool) {#getcellarea_1}

Gibt den [`CellArea`](../../cellarea/) zurück, auf den der angegebene AutoFilter angewendet wird.

```csharp
public CellArea GetCellArea(bool refreshAppliedRange)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| refreshAppliedRange | Boolean | Ob der angewendete Bereich aktualisiert werden soll. Für den angewendeten Bereich des AutoFilters kann sich die letzte Zeile ändern, wenn sich die Zellen-Daten ändern. Wenn dieses Flag true ist, wird die letzte Zeile des Bereichs anhand der aktuellen Zellen-Daten neu berechnet. |

### Rückgabewert

der Bereich, auf den dieser Filter angewendet wird

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für AutoFilter vorbereiten
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");

            // AutoFilter-Bereich festlegen (Zeile 0 bis 3, Spalte 0)
            worksheet.AutoFilter.SetRange(0, 0, 0);

            try
            {
                // GetCellArea mit refreshAppliedRange=true aufrufen
                CellArea result = worksheet.AutoFilter.GetCellArea(true);

                // Anzeige des vom AutoFilter angewendeten Bereichs
                Console.WriteLine($"AutoFilter Range: StartRow={result.StartRow}, " +
                    $"StartColumn={result.StartColumn}, EndRow={result.EndRow}, " +
                    $"EndColumn={result.EndColumn}");

                Console.WriteLine("GetCellArea method executed successfully with boolean parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("AutoFilterMethodGetCellAreaWithBooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


