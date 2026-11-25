---
title: "Worksheet.AutoFitColumns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Worksheet method. Adatta automaticamente tutte le colonne in questo foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/autofitcolumns/
---
## AutoFitColumns() {#autofitcolumns}

Adatta automaticamente tutte le colonne in questo foglio di lavoro.

```csharp
public void AutoFitColumns()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("This is a test string");
            worksheet.Cells["B1"].PutValue("Another longer test string for demonstration");
            worksheet.Cells["C1"].PutValue("Short");
            
            // Adatta automaticamente tutte le colonne nel foglio di lavoro
            worksheet.AutoFitColumns();
            
            // Salva la cartella di lavoro
            workbook.Save("AutoFitColumnsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(AutoFitterOptions) {#autofitcolumns_1}

Adatta automaticamente tutte le colonne in questo foglio di lavoro.

```csharp
public void AutoFitColumns(AutoFitterOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | AutoFitterOptions | Le opzioni di adattamento automatico |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Sample Text for AutoFit");
            worksheet.Cells["B1"].PutValue("Longer Sample Text for Testing AutoFitColumns");
            worksheet.Cells["C1"].PutValue(12345.6789);
            
            // Crea opzioni per l'adattatore automatico
            AutoFitterOptions options = new AutoFitterOptions();
            options.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            
            // Adatta le colonne con opzioni
            worksheet.AutoFitColumns(options);
            
            // Salva la cartella di lavoro
            workbook.Save("AutoFitColumnsWithOptions.xlsx");
        }
    }
}
```

### Vedi anche

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int) {#autofitcolumns_2}

Adatta automaticamente la larghezza delle colonne.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstColumn | Int32 | Indice della prima colonna. |
| lastColumn | Int32 | Indice dell'ultima colonna. |

### Osservazioni

AutoFitColumn è una funzione imprecisa.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per dimostrare l'adattamento automatico
            sheet.Cells["A1"].PutValue("Short");
            sheet.Cells["B1"].PutValue("Medium length text");
            sheet.Cells["C1"].PutValue("Very very long text that needs column width adjustment");
            sheet.Cells["D1"].PutValue("Another example with different length");

            // AutoFit colonne dall'indice 0 al 3
            sheet.AutoFitColumns(0, 3);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, AutoFitterOptions) {#autofitcolumns_3}

Adatta automaticamente la larghezza delle colonne.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstColumn | Int32 | Indice della prima colonna. |
| lastColumn | Int32 | Indice dell'ultima colonna. |
| opzioni | AutoFitterOptions | Le opzioni di adattamento automatico |

### Osservazioni

AutoFitColumn è una funzione imprecisa.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnsWithInt32Int32AutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Short text");
            worksheet.Cells["B1"].PutValue("This is a much longer text that needs column autofitting");
            worksheet.Cells["C1"].PutValue("Another example with different length");

            // Crea AutoFitterOptions con impostazioni specifiche
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
            options.IgnoreHidden = false;
            options.OnlyAuto = false;

            try
            {
                // Chiama AutoFitColumns con i parametri (firstColumn, lastColumn, options)
                worksheet.AutoFitColumns(0, 2, options);
                
                Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, AutoFitterOptions)");
                
                // Mostra l'effetto visualizzando le larghezze delle colonne
                Console.WriteLine($"Column A width: {worksheet.Cells.GetColumnWidth(0)}");
                Console.WriteLine($"Column B width: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine($"Column C width: {worksheet.Cells.GetColumnWidth(2)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, int, int) {#autofitcolumns_4}

Adatta automaticamente la larghezza delle colonne.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Indice della prima riga. |
| firstColumn | Int32 | Indice della prima colonna. |
| lastRow | Int32 | Indice dell'ultima riga. |
| lastColumn | Int32 | Indice dell'ultima colonna. |

### Osservazioni

AutoFitColumn è una funzione imprecisa.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola alcuni dati per la dimostrazione
            worksheet.Cells["A1"].PutValue("Short");
            worksheet.Cells["B1"].PutValue("Medium length text");
            worksheet.Cells["C1"].PutValue("Very very long text that needs more column width");
            
            // AutoFit colonne dalla colonna 0 (A) alla colonna 2 (C), con la prima riga 0 e l'ultima riga 0
            worksheet.AutoFitColumns(0, 2, 0, 0);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, int, int, AutoFitterOptions) {#autofitcolumns_5}

Adatta automaticamente la larghezza delle colonne.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, 
    AutoFitterOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Indice della prima riga. |
| firstColumn | Int32 | Indice della prima colonna. |
| lastRow | Int32 | Indice dell'ultima riga. |
| lastColumn | Int32 | Indice dell'ultima colonna. |
| opzioni | AutoFitterOptions | Le opzioni di adattamento automatico |

### Osservazioni

AutoFitColumn è una funzione imprecisa.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnsWithInt32Int32Int32Int32AutoFitterDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola le celle con dati di esempio che necessitano di aggiustamento della larghezza della colonna
            worksheet.Cells["A1"].PutValue("This is a long text that needs column autofit");
            worksheet.Cells["B1"].PutValue("Another lengthy text string for demonstration");
            worksheet.Cells["C1"].PutValue("Short");
            worksheet.Cells["A2"].PutValue(12345.6789);
            worksheet.Cells["B2"].PutValue("Multi-line\ntext\nsample");
            worksheet.Cells["C2"].PutValue(true);

            // Crea AutoFitterOptions con impostazioni specifiche
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
            options.IgnoreHidden = false;
            options.OnlyAuto = false;

            try
            {
                // Chiama AutoFitColumns con parametri specifici (firstRow, firstColumn, lastRow, lastColumn, options)
                worksheet.AutoFitColumns(0, 0, 1, 2, options);
                
                Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, Int32, Int32, AutoFitterOptions)");
                
                // Mostra le larghezze delle colonne dopo l'adattamento automatico
                Console.WriteLine($"Column A width after autofit: {worksheet.Cells.GetColumnWidth(0)}");
                Console.WriteLine($"Column B width after autofit: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine($"Column C width after autofit: {worksheet.Cells.GetColumnWidth(2)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


