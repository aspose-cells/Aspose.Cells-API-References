---
title: "Workbook.RefreshDynamicArrayFormulas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Aggiorna il spill delle formule di array dinamico in un nuovo intervallo di celle adiacenti in base ai dati attuali. Altre formule nel workbook non saranno calcolate ricorsivamente anche se sono state utilizzate dalle formule di array dinamico."
type: docs
url: /it/net/aspose.cells/workbook/refreshdynamicarrayformulas/
---
## RefreshDynamicArrayFormulas(bool) {#refreshdynamicarrayformulas}

Aggiorna le formule di array dinamici (si estendono in un nuovo intervallo di celle adiacenti in base ai dati attuali). Altre formule nella cartella di lavoro non saranno calcolate ricorsivamente anche se sono state utilizzate dalle formule di array dinamici.

```csharp
public void RefreshDynamicArrayFormulas(bool calculate)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| calcola | Booleano | Indica se calcola e aggiorna i valori delle celle per quelle formule di array dinamico |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet1 = wb.Worksheets[0];
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");

            // Imposta i dati iniziali e le formule di array dinamico
            sheet1.Cells["A1"].PutValue("B1:B3");
            sheet1.Cells["A2"].SetDynamicArrayFormula("=INDIRECT(A1)", new FormulaParseOptions(), true);
            sheet2.Cells["B1"].SetDynamicArrayFormula("=TRANSPOSE(Sheet1!A2#)", new FormulaParseOptions(), true);

            Console.WriteLine("Before refresh:");
            PrintSpillStatus(sheet1, sheet2);

            // Modifica l'intervallo e aggiorna le formule
            sheet1.Cells["A1"].PutValue("B1:B5");
            wb.RefreshDynamicArrayFormulas(true);

            Console.WriteLine("\nAfter refresh:");
            PrintSpillStatus(sheet1, sheet2);
        }

        private static void PrintSpillStatus(Worksheet sheet1, Worksheet sheet2)
        {
            Console.WriteLine("Sheet1 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet1.Cells.CheckCell(i, 0);
                Console.WriteLine($"Row {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
            }

            Console.WriteLine("\nSheet2 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet2.Cells.CheckCell(0, i);
                Console.WriteLine($"Column {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
            }
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshDynamicArrayFormulas(bool, CalculationOptions) {#refreshdynamicarrayformulas_1}

Aggiorna le formule di array dinamici (si estendono in un nuovo intervallo di celle adiacenti in base ai dati attuali).

```csharp
public void RefreshDynamicArrayFormulas(bool calculate, CalculationOptions copts)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| calcola | Booleano | Indica se calcola e aggiorna i valori delle celle per quelle formule di array dinamico |
| copts | CalculationOptions | Le opzioni per il calcolo delle formule |

### Osservazioni

Per motivi di prestazioni, non aggiorniamo automaticamente tutte le formule di array dinamico quando la formula stessa o i dati a cui fa riferimento cambiano. Pertanto l'utente deve chiamare questo metodo manualmente dopo le operazioni che possono influenzare le formule di array dinamico, come l'importazione/impostazione dei valori delle celle, l'inserimento/eliminazione di righe/colonne/intervalli, ecc. Per la maggior parte delle formule con funzioni, il calcolo dell'intervallo di spill richiede anche il calcolo della formula, quindi in generale è preferito il valore true per il flag "calculate". Se la formula è semplice, ad esempio un riferimento a un intervallo o un array (per esempio "=C1:E5", "={1,2;3,4}", ...), una funzione semplice su un intervallo o array (per esempio "=ABS(C1:E5)", "=1+{1,2;3,4}", ...), e tutte le formule verranno calcolate in seguito (ad esempio tramite [`CalculateFormula`](../calculateformula/)), allora utilizzare il valore false per il flag "calculate" può evitare il calcolo duplicato a beneficio delle prestazioni.

### Esempi

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanCalculationOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una formula di array dinamico di esempio
            worksheet.Cells["A1"].Formula = "=SEQUENCE(5)";
            
            // Crea le opzioni di calcolo
            CalculationOptions opts = new CalculationOptions();
            opts.CalcStackSize = 100;
            
            // Aggiorna le formule di array dinamico con le opzioni di calcolo
            workbook.RefreshDynamicArrayFormulas(true, opts);
            
            // Calcola le formule del workbook
            workbook.CalculateFormula(opts);
            
            // Restituisci il risultato da A1:A5
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].Value);
            }
        }
    }
}
```

### Vedi anche

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


