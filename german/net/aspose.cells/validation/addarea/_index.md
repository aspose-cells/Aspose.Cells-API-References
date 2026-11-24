---
title: "Validation.AddArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validation-Methode. Wendet die Validierung auf den Bereich an."
type: docs
url: /de/net/aspose.cells/validation/addarea/
---
## AddArea(CellArea) {#addarea}

Wendet die Validierung auf den Bereich an.

```csharp
public void AddArea(CellArea cellArea)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellArea | CellArea | Der Bereich. |

### Hinweise

Es ist gleichwertig, `AddArea` mit Prüfung von Schnittmenge und Rand zu verwenden.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Eine Validierung erstellen
            ValidationCollection vc = sheet.Validations;
            Validation validation = vc[vc.Add(CellArea.CreateCellArea(0, 0, 0, 0))];
            validation.Type = ValidationType.List;
            validation.Formula1 = "=A1:A10";

            // Weitere Bereiche zur Validierung hinzufügen
            for (int i = 1; i < 5; i++)
            {
                validation.AddArea(CellArea.CreateCellArea(i, 0, i, 0));
            }

            // Speichere die Arbeitsmappe
            wb.Save("ValidationMethodAddAreaWithCellAreaDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Validation with multiple areas created successfully.");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddArea(CellArea, bool, bool) {#addarea_1}

Wendet die Validierung auf den Bereich an.

```csharp
public void AddArea(CellArea cellArea, bool checkIntersection, bool checkEdge)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellArea | CellArea | Der Bereich. |
| checkIntersection | Boolean | Ob die Schnittmenge des angegebenen Bereichs mit den Bereichen vorhandener Validierungen geprüft wird. Wenn eine Validierung bereits im angegebenen Bereich (oder einem Teil davon) angewendet wurde, sollte die bestehende Validierung zuerst aus dem angegebenen Bereich entfernt werden. Andernfalls kann es zu Beschädigungen der erzeugten Validierungen kommen. Wenn der Benutzer sicher ist, dass der hinzugefügte Bereich mit keinem bestehenden Bereich überschneidet, kann dieser Parameter aus Leistungsgründen auf false gesetzt werden. |
| checkEdge | Boolean | Ob der Rand der von dieser Validierung angewendeten Bereiche geprüft wird. Die internen Einstellungen der Validierung hängen vom oberen linken Bereich ihrer angewendeten Bereiche ab; wird der angegebene Bereich zum neuen oberen linken Bereich, müssen die internen Einstellungen geändert und neu erstellt werden, sonst kann ein unerwartetes Ergebnis entstehen. Wenn der Benutzer sicher ist, dass der hinzugefügte Bereich nicht der obere linke ist, kann dieser Parameter aus Leistungsgründen auf false gesetzt werden. |

### Hinweise

In dieser Methode entfernen wir alle alten Validierungen im angegebenen Bereich. Für den oberen linken Bereich der angewendeten Bereiche einer Validation ist zuerst die StartRow die kleinste, anschließend ist die StartColumn die kleinste unter den Bereichen mit derselben kleinsten StartRow.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe und holen Sie das erste Arbeitsblatt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie eine Validierung in einem bestimmten Bereich
            Validation validation = worksheet.Validations[worksheet.Validations.Add(CellArea.CreateCellArea(5, 3, 6, 3))];
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "F3";

            // Demonstriere AddArea mit CellArea und zwei booleschen Parametern
            validation.AddArea(CellArea.CreateCellArea(3, 3, 3, 4), false, true);
            Console.WriteLine("Area count after AddArea: " + validation.Areas.Length);
            Console.WriteLine("Formula1 after AddArea: " + validation.Formula1);

            // Den hinzugefügten Bereich entfernen
            validation.RemoveArea(CellArea.CreateCellArea(3, 3, 3, 4));
            Console.WriteLine("Area count after RemoveArea: " + validation.Areas.Length);

            // Mehrere Bereiche mit einer Massenoperation hinzufügen
            CellArea[] areas = new CellArea[10];
            for (int i = 0; i < areas.Length; i++)
            {
                areas[i] = CellArea.CreateCellArea(6 + i, 3, 6 + i, 4);
            }
            validation.AddAreas(areas, true, true);
            Console.WriteLine("Area count after bulk AddAreas: " + validation.Areas.Length);

            // Speichere die Arbeitsmappe
            workbook.Save("ValidationMethodAddAreaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


