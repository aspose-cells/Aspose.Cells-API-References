---
title: "Workbook.CalculateFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Calcola il risultato delle formule"
type: docs
url: /it/net/aspose.cells/workbook/calculateformula/
---
## CalculateFormula() {#calculateformula}

Calcola il risultato delle formule.

```csharp
public void CalculateFormula()
```

### Osservazioni

Per tutte le formule supportate, consultare l'elenco all'indirizzo https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Imposta valori e formule
            cells["A1"].PutValue(5);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=B1+10";
            
            // Calcola le formule
            workbook.CalculateFormula();
            
            // Visualizza i risultati
            Console.WriteLine("A1 value: " + cells["A1"].IntValue);
            Console.WriteLine("B1 formula result: " + cells["B1"].IntValue);
            Console.WriteLine("C1 formula result: " + cells["C1"].IntValue);
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(bool) {#calculateformula_2}

Calcola il risultato delle formule.

```csharp
public void CalculateFormula(bool ignoreError)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ignoreError | Booleano | Indica se nascondere l'errore nel calcolo delle formule. L'errore può essere una funzione non supportata, collegamenti esterni, ecc. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaWithBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Accedi al primo foglio di lavoro e alle sue celle
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Inserisci valori nella prima riga (A1:E1)
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(i + 1); // Values 1-5
            }

            // Inserisci valori nella seconda riga (A2:E2)
            for (int i = 0; i < 5; i++)
            {
                cells[1, i].PutValue((i + 1) * 10); // Values 10,20,30,40,50
            }

            // Imposta una formula HLOOKUP condivisa nella quarta riga (A4:E4)
            cells[3, 0].SetSharedFormula("=HLOOKUP(A1,$A$1:$E$2,2,FALSE)", 1, 5);

            // Calcola le formule senza calcolo ricorsivo
            wb.CalculateFormula(false);

            // Visualizza i risultati
            Console.WriteLine("Formula calculation results:");
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Cell {((char)('A' + i))}4 value: {cells[3, i].StringValue}");
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

## CalculateFormula(CalculationOptions) {#calculateformula_1}

Calcolo delle formule in questa cartella di lavoro.

```csharp
public void CalculateFormula(CalculationOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | CalculationOptions | Opzioni per il calcolo |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaWithCalculationOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Crea una tabella e imposta i nomi delle colonne
            sheet.Cells["A1"].PutValue("A");
            sheet.Cells["B1"].PutValue("B");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(2);
            
            // Imposta formule e calcola
            Cells cells = sheet.Cells;
            cells["C1"].PutValue("InvalidColumn");
            cells["D1"].Formula = "=INDIRECT(\"A\"&ROW())";
            cells["E1"].Formula = "=IFERROR(INDIRECT(\"B\"&ROW()),\"OK\")";
            
            // Calcola le formule con opzioni
            wb.CalculateFormula(new CalculationOptions());
            
            // Restituisci i risultati
            Console.WriteLine("D1 result: " + cells["D1"].StringValue);
            Console.WriteLine("E1 result: " + cells["E1"].StringValue);
        }
    }
}
```

### Vedi anche

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


