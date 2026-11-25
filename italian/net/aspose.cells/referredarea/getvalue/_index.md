---
title: "ReferredArea.GetValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ReferredArea. Ottiene il valore della cella con l'offset specificato dall'angolo superiore sinistro di quest'area"
type: docs
url: /it/net/aspose.cells/referredarea/getvalue/
---
## GetValue(int, int) {#getvalue}

Ottiene il valore della cella con l'offset specificato dall'angolo in alto a sinistra di quest'area.

```csharp
public object GetValue(int rowOffset, int colOffset)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | Int32 | offset di riga dall'inizio della riga di quest'area |
| colOffset | Int32 | offset di colonna dall'inizio della riga di quest'area |

### Valore di ritorno

"#REF!" se quest'area è non valida; "#N/A" se l'offset fornito è fuori da quest'area; altrimenti restituisce il valore della cella nella posizione specificata.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValueWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue(5);
            Cell cell = worksheet.Cells["C1"];
            cell.Formula = "=A1";
            
            workbook.CalculateFormula();
            
            ReferredAreaCollection referredAreas = cell.GetPrecedents();
            if (referredAreas.Count > 0)
            {
                object value = referredAreas[0].GetValue(0, 0);
                Console.WriteLine("Value at (0,0): " + value);
            }
        }
    }
}
```

### Vedi anche

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetValue(int, int, bool) {#getvalue_1}

Ottiene il valore della cella con l'offset specificato dall'angolo in alto a sinistra di quest'area.

```csharp
public object GetValue(int rowOffset, int colOffset, bool calculateFormulas)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | Int32 | offset di riga dall'inizio della riga di quest'area |
| colOffset | Int32 | offset di colonna dall'inizio della riga di quest'area |
| calculateFormulas | Booleano | Se calcolarlo ricorsivamente se il riferimento specificato è una formula |

### Valore di ritorno

"#REF!" se quest'area è non valida; "#N/A" se l'offset fornito è fuori da quest'area; altrimenti restituisce il valore della cella nella posizione specificata.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue(100);
            sheet.Cells["B1"].PutValue(200);

            workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names["TestRange"];
            name.RefersTo = "=Sheet1!$A$1:$B$1";

            ReferredArea ra = name.GetReferredAreas(true)[0];
            object result = ra.GetValue(0, 0, true);

            Console.WriteLine("Obtained value: " + result);
        }
    }
}
```

### Vedi anche

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


