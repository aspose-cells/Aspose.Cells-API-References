---
title: "UnionRange.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà UnionRange. Ottiene o imposta il nome dell'intervallo"
type: docs
url: /it/net/aspose.cells/unionrange/name/
---
## UnionRange.Name property

Ottiene o imposta il nome dell'intervallo.

```csharp
public string Name { get; set; }
```

### Osservazioni

Gli intervalli denominati sono supportati. Ad esempio,

range.Name = "Sheet1!MyRange";

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].Value = "First Range";
            worksheet.Cells["B2"].Value = "Second Range";

            try
            {
                // Crea intervalli e combinali in un intervallo di unione
                Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:A1");
                Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:B2");
                UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

                // Visualizza il valore corrente della proprietà Name
                Console.WriteLine("Initial Name value: " + unionRange.Name);

                // Imposta un nuovo nome per l'intervallo UnionRange
                unionRange.Name = "MyUnionRange";
                Console.WriteLine("Updated Name value: " + unionRange.Name);

                // Dimostra che il nome può essere cambiato nuovamente
                unionRange.Name = "CustomUnionRange";
                Console.WriteLine("Final Name value: " + unionRange.Name);

                // Salva la cartella di lavoro
                workbook.Save("UnionRangeNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


