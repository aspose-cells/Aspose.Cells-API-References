---
title: "Worksheet.AutoFitRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Adatta automaticamente tutte le righe in questo foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/autofitrows/
---
## AutoFitRows(AutoFitterOptions) {#autofitrows_1}

Adatta automaticamente tutte le righe in questo foglio di lavoro.

```csharp
public void AutoFitRows(AutoFitterOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | AutoFitterOptions | Le opzioni dell'auto adattatore |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta dati di esempio e formattazione
            worksheet.Cells["A1"].PutValue("This is a long text that will need auto-fitting");
            worksheet.Cells["A2"].PutValue("Another long text\nwith multiple lines\nfor demonstration");
            
            // Unisci le celle per dimostrare l'adattamento automatico delle celle unite
            worksheet.Cells.Merge(3, 0, 2, 1);
            worksheet.Cells["A3"].PutValue("Merged cells text that needs to fit");

            // Adatta automaticamente le righe con opzioni specifiche
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                MaxRowHeight = 100,  // Set reasonable max height
                OnlyAuto = true
            });

            // Salva la cartella di lavoro
            workbook.Save("AutoFitRowsDemo.xlsx");
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

## AutoFitRows(int, int) {#autofitrows_3}

Adatta automaticamente l'altezza della riga in un intervallo.

```csharp
public void AutoFitRows(int startRow, int endRow)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Indice della riga iniziale. |
| endRow | Int32 | Indice della riga finale. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Popola le celle con dati di esempio e stili
            for (int i = 0; i <= 8; i++)
            {
                Cell cell = cells[i, i];
                cell.Value = "Sample text for row " + i;
                
                if (i % 2 == 0)
                {
                    Style style = cell.GetStyle();
                    style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, System.Drawing.Color.Black);
                    cell.SetStyle(style);
                }
            }

            // Adatta automaticamente le righe dall'indice 0 all'8
            sheet.AutoFitRows(0, 8);

            // Restituisci le altezze delle righe risultanti
            for (int i = 0; i <= 8; i++)
            {
                Console.WriteLine($"Row {i} height: {cells.GetRowHeightPixel(i)} pixels");
            }
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(int, int, AutoFitterOptions) {#autofitrows_4}

Adatta automaticamente l'altezza della riga in un intervallo.

```csharp
public void AutoFitRows(int startRow, int endRow, AutoFitterOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Indice della riga iniziale. |
| endRow | Int32 | Indice della riga finale. |
| opzioni | AutoFitterOptions | Le opzioni dell'adattatore automatico. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithInt32Int32AutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("This is a test string for auto-fit row height demonstration");
            worksheet.Cells["A2"].PutValue("Another line\nwith multiple lines\nof text");
            
            // Crea opzioni per l'adattatore automatico
            AutoFitterOptions options = new AutoFitterOptions();
            options.OnlyAuto = true;
            
            // Adatta automaticamente le righe da 0 a 1 con opzioni
            worksheet.AutoFitRows(0, 1, options);
            
            // Salva la cartella di lavoro
            workbook.Save("AutoFitRowsDemo.xlsx");
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

## AutoFitRows() {#autofitrows}

Adatta automaticamente tutte le righe in questo foglio di lavoro.

```csharp
public void AutoFitRows()
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("This is a test string for AutoFitRows demonstration");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line break to show row height adjustment");
            worksheet.Cells["B1"].PutValue("Column B content");
            
            // Adatta automaticamente le righe
            worksheet.AutoFitRows();
            
            // Adatta automaticamente le colonne per una migliore visibilità
            worksheet.AutoFitColumns();
            
            // Salva la cartella di lavoro
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "AutoFitRowsDemo.xlsx");
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Worksheet with AutoFitRows saved to: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(bool) {#autofitrows_2}

Adatta automaticamente tutte le righe in questo foglio di lavoro.

```csharp
public void AutoFitRows(bool onlyAuto)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| onlyAuto | Booleano | True,adatta automaticamente l'altezza della riga solo quando l'altezza della riga non è personalizzata. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi testo di esempio alle celle per dimostrare l'adattamento automatico delle righe
            worksheet.Cells["A1"].PutValue("This is a sample text that will demonstrate AutoFitRows functionality");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line breaks\nto show multi-line row adjustment");
            
            // Adatta automaticamente le righe tenendo conto dell'unione automatica
            worksheet.AutoFitRows(true);
            
            // Salva la cartella di lavoro
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


