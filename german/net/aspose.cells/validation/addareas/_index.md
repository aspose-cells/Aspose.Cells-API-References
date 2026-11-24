---
title: "Validation.AddAreas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validation-Methode. Wendet die Validierung auf die angegebenen Bereiche an"
type: docs
url: /de/net/aspose.cells/validation/addareas/
---
## Validation.AddAreas method

Wendet die Validierung auf die angegebenen Bereiche an.

```csharp
public void AddAreas(CellArea[] areas, bool checkIntersection, bool checkEdge)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereiche | CellArea[] | Die Bereiche. |
| checkIntersection | Boolean | Ob die Schnittmenge des angegebenen Bereichs mit den Bereichen bestehender Validierungen überprüft wird. Wenn bereits eine Validierung im angegebenen Bereich (oder einem Teil davon) angewendet wurde, sollte die bestehende Validierung zunächst aus dem angegebenen Bereich entfernt werden. Andernfalls kann es zu Beschädigungen der erzeugten Validierungen kommen. Wenn der Benutzer sicher ist, dass alle hinzugefügten Bereiche nicht mit einem bestehenden Bereich überschneiden, kann dieser Parameter aus Leistungsgründen auf false gesetzt werden. |
| checkEdge | Boolean | Ob die Kante der angewendeten Bereiche dieser Validierung überprüft wird. Die internen Einstellungen der Validierung hängen vom oberen linken Bereich ihrer angewendeten Bereiche ab, sodass, wenn einer der angegebenen Bereiche zum neuen oberen linken Bereich der angewendeten Bereiche wird, die internen Einstellungen geändert und neu erstellt werden müssen, andernfalls können unerwartete Ergebnisse auftreten. Wenn der Benutzer sicher ist, dass keiner der hinzugefügten Bereiche der obere linke ist, kann dieser Parameter aus Leistungsgründen auf false gesetzt werden. |

### Hinweise

In dieser Methode entfernen wir alle alten Validierungen im angegebenen Bereich. Für den oberen linken Bereich der angewendeten Bereiche einer Validation ist zuerst die StartRow die kleinste, anschließend ist die StartColumn die kleinste unter den Bereichen mit derselben kleinsten StartRow.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodAddAreasWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int validationIndex = worksheet.Validations.Add();
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.List;
            validation.AlertStyle = ValidationAlertType.Stop;
            validation.Operator = OperatorType.None;
            validation.Formula1 = "1,2,3";
            validation.InCellDropDown = true;

            CellArea[] areas = new CellArea[2];
            areas[0] = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 1 };
            areas[1] = new CellArea { StartRow = 2, StartColumn = 2, EndRow = 3, EndColumn = 3 };

            try
            {
                validation.AddAreas(areas, true, false);
                Console.WriteLine("Added validation areas with checkIntersection=true, checkEdge=false");

                foreach (CellArea area in validation.Areas)
                {
                    Console.WriteLine($"Validation area: R{area.StartRow + 1}C{area.StartColumn + 1}:R{area.EndRow + 1}C{area.EndColumn + 1}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding validation areas: {ex.Message}");
            }

            workbook.Save("ValidationAddAreasDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


