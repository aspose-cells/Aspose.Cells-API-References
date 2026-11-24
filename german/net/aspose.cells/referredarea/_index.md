---
title: "Klasse ReferredArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ReferredArea Klasse. Stellt einen durch die Formel referenzierten Bereich dar"
type: docs
url: /de/net/aspose.cells/referredarea/
---
## ReferredArea class

Stellt einen von der Formel referenzierten Bereich dar.

```csharp
public class ReferredArea
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [EndColumn](../../aspose.cells/referredarea/endcolumn/) { get; } | Die Endspalte des Bereichs. |
| [EndRow](../../aspose.cells/referredarea/endrow/) { get; } | Die Endzeile des Bereichs. |
| [ExternalFileName](../../aspose.cells/referredarea/externalfilename/) { get; } | Den externen Dateinamen abrufen, wenn dies eine externe Referenz ist. |
| [IsArea](../../aspose.cells/referredarea/isarea/) { get; } | Gibt an, ob dies ein Bereich ist. |
| [IsEntireColumn](../../aspose.cells/referredarea/isentirecolumn/) { get; } | Gibt an, ob dieser Bereich alle Zeilen (gesamte Spalte) enthält. |
| [IsEntireRow](../../aspose.cells/referredarea/isentirerow/) { get; } | Gibt an, ob dieser Bereich alle Spalten (gesamte Zeile) enthält. |
| [IsExternalLink](../../aspose.cells/referredarea/isexternallink/) { get; } | Gibt an, ob dies ein externer Link ist. |
| [SheetName](../../aspose.cells/referredarea/sheetname/) { get; } | Gibt an, in welchem Blatt diese Referenz ist. |
| [SheetNames](../../aspose.cells/referredarea/sheetnames/) { get; } | Namen aller Arbeitsblätter, auf die diese Instanz verweist. |
| [StartColumn](../../aspose.cells/referredarea/startcolumn/) { get; } | Die Startspalte des Bereichs. |
| [StartRow](../../aspose.cells/referredarea/startrow/) { get; } | Die Startzeile des Bereichs. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue)(int, int) | Ermittelt den Zellenwert mit dem angegebenen Versatz von der oberen linken Ecke dieses Bereichs. |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue_1)(int, int, bool) | Ermittelt den Zellenwert mit dem angegebenen Versatz von der oberen linken Ecke dieses Bereichs. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues)() | Ermittelt Zellwerte in diesem Bereich. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues_1)(bool) | Ermittelt Zellwerte in diesem Bereich. |
| override [ToString](../../aspose.cells/referredarea/tostring/)() | Gibt die Referenzadresse dieses Bereichs zurück. In der Regel ist dies die Adresse der Referenz, die in einer Formel verwendet werden kann, z. B. "Sheet1!A1:C3". |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassReferredAreaDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Richten Sie einige Daten und eine Formel ein, die einen Bereich referenziert
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["B1"].PutValue(30);
                worksheet.Cells["B2"].PutValue(40);

                // Erstellen Sie eine Formel, die den Bereich A1:B2 referenziert
                Cell formulaCell = worksheet.Cells["C1"];
                formulaCell.Formula = "=SUM(A1:B2)";

                // Rufen Sie die referenzierten Bereiche aus der Formel ab
                ReferredAreaCollection referredAreas = formulaCell.GetPrecedents();
                if (referredAreas.Count > 0)
                {
                    // Rufen Sie den ersten referenzierten Bereich ab
                    ReferredArea referredArea = referredAreas[0];

                    // Zeigen Sie grundlegende Eigenschaften des referenzierten Bereichs an
                    Console.WriteLine($"Referred Area Details:");
                    Console.WriteLine($"- Is External Link: {referredArea.IsExternalLink}");
                    Console.WriteLine($"- Sheet Name: {referredArea.SheetName}");
                    Console.WriteLine($"- Start Row: {referredArea.StartRow}");
                    Console.WriteLine($"- Start Column: {referredArea.StartColumn}");
                    Console.WriteLine($"- End Row: {referredArea.EndRow}");
                    Console.WriteLine($"- End Column: {referredArea.EndColumn}");
                    Console.WriteLine($"- Is Area: {referredArea.IsArea}");
                    Console.WriteLine($"- Is Entire Row: {referredArea.IsEntireRow}");
                    Console.WriteLine($"- Is Entire Column: {referredArea.IsEntireColumn}");

                    // Werte aus dem referenzierten Bereich abrufen
                    object values = referredArea.GetValues();
                    if (values is Array)
                    {
                        object[][] valueArray = (object[][])values;
                        Console.WriteLine("\nValues in the referred area:");
                        foreach (object[] row in valueArray)
                        {
                            foreach (object val in row)
                            {
                                Console.Write($"{val}\t");
                            }
                            Console.WriteLine();
                        }
                    }

                    // Einen bestimmten Wert aus dem referenzierten Bereich abrufen
                    object specificValue = referredArea.GetValue(0, 1);
                    Console.WriteLine($"\nValue at row 0, column 1: {specificValue}");

                    // Anzeige der Referenzadresse
                    Console.WriteLine($"Reference address: {referredArea.ToString()}");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("ReferredAreaDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ReferredArea: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


