---
title: "Classe ReferredArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ReferredArea classe. Rappresenta un'area di riferimento tramite la formula"
type: docs
url: /it/net/aspose.cells/referredarea/
---
## ReferredArea class

Rappresenta un'area di riferimento della formula.

```csharp
public class ReferredArea
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [EndColumn](../../aspose.cells/referredarea/endcolumn/) { get; } | La colonna finale dell'area. |
| [EndRow](../../aspose.cells/referredarea/endrow/) { get; } | La riga finale dell'area. |
| [ExternalFileName](../../aspose.cells/referredarea/externalfilename/) { get; } | Ottieni il nome del file esterno se si tratta di un riferimento esterno. |
| [IsArea](../../aspose.cells/referredarea/isarea/) { get; } | Indica se si tratta di un'area. |
| [IsEntireColumn](../../aspose.cells/referredarea/isentirecolumn/) { get; } | Indica se quest'area contiene tutte le righe (intera colonna). |
| [IsEntireRow](../../aspose.cells/referredarea/isentirerow/) { get; } | Indica se quest'area contiene tutte le colonne (intera riga). |
| [IsExternalLink](../../aspose.cells/referredarea/isexternallink/) { get; } | Indica se questo è un collegamento esterno. |
| [SheetName](../../aspose.cells/referredarea/sheetname/) { get; } | Indica in quale foglio si trova questo riferimento. |
| [SheetNames](../../aspose.cells/referredarea/sheetnames/) { get; } | Nomi di tutti i fogli di lavoro a cui fa riferimento questa istanza. |
| [StartColumn](../../aspose.cells/referredarea/startcolumn/) { get; } | La colonna iniziale dell'area. |
| [StartRow](../../aspose.cells/referredarea/startrow/) { get; } | La riga iniziale dell'area. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue)(int, int) | Ottiene il valore della cella con l'offset specificato dall'angolo in alto a sinistra di quest'area. |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue_1)(int, int, bool) | Ottiene il valore della cella con l'offset specificato dall'angolo in alto a sinistra di quest'area. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues)() | Ottiene i valori delle celle in quest'area. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues_1)(bool) | Ottiene i valori delle celle in quest'area. |
| override [ToString](../../aspose.cells/referredarea/tostring/)() | Restituisce l'indirizzo di riferimento di quest'area. Generalmente è l'indirizzo del riferimento che può essere usato in una formula, ad esempio "Sheet1!A1:C3". |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassReferredAreaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Imposta alcuni dati e una formula che fa riferimento a un intervallo
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["B1"].PutValue(30);
                worksheet.Cells["B2"].PutValue(40);

                // Crea una formula che fa riferimento all'intervallo A1:B2
                Cell formulaCell = worksheet.Cells["C1"];
                formulaCell.Formula = "=SUM(A1:B2)";

                // Ottieni le aree di riferimento dalla formula
                ReferredAreaCollection referredAreas = formulaCell.GetPrecedents();
                if (referredAreas.Count > 0)
                {
                    // Ottieni la prima area di riferimento
                    ReferredArea referredArea = referredAreas[0];

                    // Visualizza le proprietà di base dell'area di riferimento
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

                    // Ottieni i valori dall'area di riferimento
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

                    // Ottieni un valore specifico dall'area di riferimento
                    object specificValue = referredArea.GetValue(0, 1);
                    Console.WriteLine($"\nValue at row 0, column 1: {specificValue}");

                    // Visualizza l'indirizzo di riferimento
                    Console.WriteLine($"Reference address: {referredArea.ToString()}");
                }

                // Salva la cartella di lavoro
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

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


