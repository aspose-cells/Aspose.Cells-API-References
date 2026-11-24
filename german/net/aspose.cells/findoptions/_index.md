---
title: "Klasse FindOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FindOptions Klasse. Stellt Suchoptionen dar"
type: docs
url: /de/net/aspose.cells/findoptions/
---
## FindOptions class

Stellt Suchoptionen dar.

```csharp
public class FindOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [FindOptions](findoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CaseSensitive](../../aspose.cells/findoptions/casesensitive/) { get; set; } | Gibt an, ob die gesuchte Zeichenfolge Groß‑ und Kleinschreibung beachtet. |
| [ConvertNumericData](../../aspose.cells/findoptions/convertnumericdata/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob der gesuchte Zeichenfolgenwert in numerische Daten konvertiert wird. |
| [IsCaseSensitive](../../aspose.cells/findoptions/iscasesensitive/) { get; set; } | (**Obsolete.**) Gibt an, ob die gesuchte Zeichenfolge Groß‑ und Kleinschreibung beachtet. |
| [IsRangeSet](../../aspose.cells/findoptions/israngeset/) { get; } | Gibt an, ob der gesuchte Bereich festgelegt ist. |
| [LookAtType](../../aspose.cells/findoptions/lookattype/) { get; set; } | Typ ansehen. |
| [LookInType](../../aspose.cells/findoptions/lookintype/) { get; set; } | Im Typ nachsehen. |
| [RegexKey](../../aspose.cells/findoptions/regexkey/) { get; set; } | Gibt an, ob der gesuchte Schlüssel ein Regex ist. Wenn true, wird der gesuchte Schlüssel als Regex behandelt und geparst. Andernfalls wird der Schlüssel gemäß den Regeln in MS Excel geparst. |
| [SearchBackward](../../aspose.cells/findoptions/searchbackward/) { get; set; } | Ob rückwärts nach Zellen gesucht werden soll. |
| [SearchNext](../../aspose.cells/findoptions/searchnext/) { get; set; } | (**Obsolete.**) Suchreihenfolge. True: nächstes suchen. False: vorheriges suchen. |
| [SearchOrderByRows](../../aspose.cells/findoptions/searchorderbyrows/) { get; set; } | Gibt an, ob die Suchreihenfolge nach Zeilen oder Spalten erfolgt. |
| [Style](../../aspose.cells/findoptions/style/) { get; set; } | Das zu suchende Format. |
| [ValueTypeSensitive](../../aspose.cells/findoptions/valuetypesensitive/) { get; set; } | Gibt an, ob der Typ des gesuchten Zellwerts mit dem gesuchten Schlüssel übereinstimmen soll. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetRange](../../aspose.cells/findoptions/getrange/)() | Liest und setzt den zu suchenden Bereich. |
| [SetRange](../../aspose.cells/findoptions/setrange/)(CellArea) | Setzt den zu suchenden Bereich. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsDemo
    {
        public static void FindOptionsExample()
        {
            // Instanziieren Sie das Arbeitsmappen-Objekt
            Workbook workbook = new Workbook("FindOptionsExample_original.xlsx");

            // Abrufen der Zellen-Sammlung
            Cells cells = workbook.Worksheets[0].Cells;

            // Instanziieren Sie das FindOptions-Objekt
            FindOptions findOptions = new FindOptions();

            // Erstellen Sie einen Zellenbereich
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.StartColumn = 0;
            ca.EndRow = 5;
            ca.EndColumn = 5;

            // Legen Sie den Zellenbereich für FindOptions fest
            findOptions.SetRange(ca);

            // Such-Eigenschaften festlegen
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // Finde die Zelle mit dem Wert 0
            Cell cell = cells.Find(0, null, findOptions);

            if (cell != null)
            {
                Console.WriteLine("Cell found at: " + cell.Name);
            }
            else
            {
                Console.WriteLine("Cell not found.");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


