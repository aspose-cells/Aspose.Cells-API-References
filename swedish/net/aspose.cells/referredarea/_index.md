---
title: "Klass ReferredArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ReferredArea klass. Representerar ett refererat område enligt formeln"
type: docs
url: /sv/net/aspose.cells/referredarea/
---
## ReferredArea class

Representerar ett refererat område enligt formeln.

```csharp
public class ReferredArea
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [EndColumn](../../aspose.cells/referredarea/endcolumn/) { get; } | Slutkolumnen för området. |
| [EndRow](../../aspose.cells/referredarea/endrow/) { get; } | Slutraden för området. |
| [ExternalFileName](../../aspose.cells/referredarea/externalfilename/) { get; } | Hämta det externa filnamnet om detta är en extern referens. |
| [IsArea](../../aspose.cells/referredarea/isarea/) { get; } | Indikerar om detta är ett område. |
| [IsEntireColumn](../../aspose.cells/referredarea/isentirecolumn/) { get; } | Indikerar om detta område innehåller alla rader (hela kolumnen). |
| [IsEntireRow](../../aspose.cells/referredarea/isentirerow/) { get; } | Indikerar om detta område innehåller alla kolumner (hela raden). |
| [IsExternalLink](../../aspose.cells/referredarea/isexternallink/) { get; } | Indikerar om detta är en extern länk. |
| [SheetName](../../aspose.cells/referredarea/sheetname/) { get; } | Indikerar vilket blad denna referens finns i. |
| [SheetNames](../../aspose.cells/referredarea/sheetnames/) { get; } | Namn på alla kalkylblad som denna instans refererar till. |
| [StartColumn](../../aspose.cells/referredarea/startcolumn/) { get; } | Startkolumnen för området. |
| [StartRow](../../aspose.cells/referredarea/startrow/) { get; } | Startraden för området. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue)(int, int) | Hämtar cellvärdet med given offset från det övre vänstra hörnet av detta område. |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue_1)(int, int, bool) | Hämtar cellvärdet med given offset från det övre vänstra hörnet av detta område. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues)() | Hämtar cellvärden i detta område. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues_1)(bool) | Hämtar cellvärden i detta område. |
| override [ToString](../../aspose.cells/referredarea/tostring/)() | Returnerar referensadressen för detta område. Vanligtvis är det referensens adress som kan användas i en formel, till exempel "Sheet1!A1:C3". |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassReferredAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ställ in lite data och en formel som refererar till ett område
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["B1"].PutValue(30);
                worksheet.Cells["B2"].PutValue(40);

                // Skapa en formel som refererar till området A1:B2
                Cell formulaCell = worksheet.Cells["C1"];
                formulaCell.Formula = "=SUM(A1:B2)";

                // Hämta de refererade områdena från formeln
                ReferredAreaCollection referredAreas = formulaCell.GetPrecedents();
                if (referredAreas.Count > 0)
                {
                    // Hämta det första refererade området
                    ReferredArea referredArea = referredAreas[0];

                    // Visa grundläggande egenskaper för det refererade området
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

                    // Hämta värden från det refererade området
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

                    // Hämta ett specifikt värde från det refererade området
                    object specificValue = referredArea.GetValue(0, 1);
                    Console.WriteLine($"\nValue at row 0, column 1: {specificValue}");

                    // Visa referensadressen
                    Console.WriteLine($"Reference address: {referredArea.ToString()}");
                }

                // Spara arbetsboken
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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


