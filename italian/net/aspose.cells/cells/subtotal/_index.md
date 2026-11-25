---
title: "Cells.Subtotal"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Crea subtotali per l'intervallo"
type: docs
url: /it/net/aspose.cells/cells/subtotal/
---
## Subtotal(CellArea, int, ConsolidationFunction, int[]) {#subtotal}

Crea subtotali per l'intervallo.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | CellArea | L'intervallo |
| groupBy | Int32 | Il campo per il raggruppamento, come offset intero a base zero |
| funzione | ConsolidationFunction | La funzione di subtotale. |
| totalList | Int32[] | Un array di offset di campo basati su zero, che indica i campi a cui vengono aggiunti i subtotali. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola dati di esempio per il subtotale
            CreateSampleData(worksheet);

            // Definisci l'area di celle contenente i dati (A1:C6)
            CellArea cellArea = CellArea.CreateCellArea(0, 0, 5, 2);

            try
            {
                // Chiama il metodo Subtotal con i parametri:
                // - Raggruppa per colonna 0 (Regione)
                // - Usa la funzione SOMMA
                // - Applica alla colonna 2 (Vendite)
                worksheet.Cells.Subtotal(
                    cellArea,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 }
                );

                Console.WriteLine("Subtotal added successfully for parameters (CellArea, 0, Sum, [2])");
                
                // I metodi ExpandColumnLevel e ExpandRowLevel sono stati rimossi per correggere gli errori di compilazione
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Subtotal method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Crea la riga di intestazione
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["C1"].PutValue("Sales");

            // Crea le righe di dati
            object[,] data = new object[,] {
                {"North", "Widget", 5000},
                {"North", "Gadget", 3000},
                {"South", "Widget", 6000},
                {"South", "Gadget", 4000},
                {"West", "Widget", 4500}
            };

            // Popola i dati a partire dalla riga 2 (indice basato su zero 1)
            for (int i = 0; i < data.GetLength(0); i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(data[i, 0]);
                worksheet.Cells[i + 1, 1].PutValue(data[i, 1]);
                worksheet.Cells[i + 1, 2].PutValue(data[i, 2]);
            }
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Subtotal(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) {#subtotal_1}

Crea subtotali per l'intervallo.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList, 
    bool replace, bool pageBreaks, bool summaryBelowData)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | CellArea | L'intervallo |
| groupBy | Int32 | Il campo per il raggruppamento, come offset intero a base zero |
| funzione | ConsolidationFunction | La funzione di subtotale. |
| totalList | Int32[] | Un array di offset di campo basati su zero, che indica i campi a cui vengono aggiunti i subtotali. |
| sostituisci | Booleano | Indica se sostituire i subtotali correnti |
| pageBreaks | Booleano | Indica se aggiungere un'interruzione di pagina tra i gruppi |
| summaryBelowData | Booleano | Indica se aggiungere il riepilogo sotto i dati. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea dati di esempio per il subtotale
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            object[,] data = new object[,] {
                { "Fruits", "Apple", 1500 },
                { "Fruits", "Orange", 2500 },
                { "Vegetables", "Carrot", 1800 },
                { "Vegetables", "Potato", 3000 },
                { "Fruits", "Banana", 2000 }
            };

            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    cells[row + 1, col].PutValue(data[row, col]);
                }
            }

            try
            {
                // Definisci l'area di celle per il subtotale (A1:C6)
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 5;
                area.EndColumn = 2;

                // Chiama Subtotal con i parametri:
                // - Raggruppa per la prima colonna (indice basato su zero 0)
                // - Usa la funzione Somma
                // - Applica alla terza colonna (indice basato su zero 2)
                // - Sostituisci i subtotali esistenti, interruzioni di pagina tra i gruppi, riepilogo sotto i dati
                cells.Subtotal(
                    area,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 },
                    true,
                    true,
                    true
                );

                Console.WriteLine("Subtotal added successfully for parameters: (CellArea, Int32, ConsolidationFunction, Int32[], Boolean, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating subtotal: {ex.Message}");
            }

            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


