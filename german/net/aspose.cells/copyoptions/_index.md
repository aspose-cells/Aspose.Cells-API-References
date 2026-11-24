---
title: "Klasse CopyOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CopyOptions Klasse. Stellt die Kopieroptionen dar"
type: docs
url: /de/net/aspose.cells/copyoptions/
---
## CopyOptions class

Stellt die Kopieroptionen dar.

```csharp
public class CopyOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [CopyOptions](copyoptions/)() | CopyOptions-Konstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ColumnCharacterWidth](../../aspose.cells/copyoptions/columncharacterwidth/) { get; set; } | Gibt an, ob die Spaltenbreite in Zeichen als Einheit kopiert wird. |
| [CopyInvalidFormulasAsValues](../../aspose.cells/copyoptions/copyinvalidformulasasvalues/) { get; set; } | Wenn die Formel für das Ziel nicht gültig ist, werden nur Werte kopiert. |
| [CopyNames](../../aspose.cells/copyoptions/copynames/) { get; set; } | Gibt an, ob die Namen kopiert werden. |
| [ExtendToAdjacentRange](../../aspose.cells/copyoptions/extendtoadjacentrange/) { get; set; } | Gibt an, ob Bereiche erweitert werden, wenn der Bereich in einen angrenzenden Bereich kopiert wird. |
| [KeepMacros](../../aspose.cells/copyoptions/keepmacros/) { get; set; } | Gibt an, ob Makros beibehalten werden; |
| [ReferToDestinationSheet](../../aspose.cells/copyoptions/refertodestinationsheet/) { get; set; } | Beim Kopieren des Bereichs in derselben Datei und wenn das Diagramm auf das Quellblatt verweist, bedeutet False, dass die Datenquelle des kopierten Diagramms nicht geändert wird. True bedeutet, dass die Datenquelle des kopierten Diagramms auf das Zielblatt verweist. |
| [ReferToSheetWithSameName](../../aspose.cells/copyoptions/refertosheetwithsamename/) { get; set; } | In MS Excel, wenn Formeln, die sich auf andere Arbeitsblätter beziehen, beim Kopieren eines Arbeitsblatts in ein anderes kopiert werden, sollten die kopierten Formeln auf die Quellarbeitsmappe verweisen. In einigen Situationen muss der Benutzer jedoch, dass die kopierten Formeln auf Arbeitsblätter mit demselben Namen in derselben Arbeitsmappe verweisen, zum Beispiel wenn diese Arbeitsblätter bereits vor diesem Kopiervorgang kopiert wurden; dann sollte diese Eigenschaft auf true gesetzt bleiben. |
| [UpdateInvalidReferencesToTargetSheet](../../aspose.cells/copyoptions/updateinvalidreferencestotargetsheet/) { get; set; } | Gibt an, ob auf das Zielarbeitsblatt verwiesen werden soll, wenn das referenzierte Arbeitsblatt nicht kopiert wurde. |

### Beispiele

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CopyOptionsDemo
    {
        public static void CopyOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");

            // Erstelle ein neues Arbeitsbuch, in das Daten kopiert werden sollen
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // Erstelle ein CopyOptions-Objekt
            CopyOptions copyOptions = new CopyOptions
            {
                KeepMacros = true,
                ExtendToAdjacentRange = true,
                CopyNames = true,
                CopyInvalidFormulasAsValues = true,
                ColumnCharacterWidth = true,
                ReferToSheetWithSameName = true,
                ReferToDestinationSheet = true
            };

            // Kopiere die Daten vom Quellarbeitsblatt zum Zielarbeitsblatt
            destSheet.Cells.CopyRows(sheet.Cells, 0, 0, 2, copyOptions);

            // Speichere das Zielarbeitsbuch
            destWorkbook.Save("CopyOptionsExample.xlsx");
            destWorkbook.Save("CopyOptionsExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


