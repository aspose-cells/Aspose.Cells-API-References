---
title: "Workbook.GetStyleInPool"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Ottiene lo stile nel pool di stili. Tutti gli stili nel workbook verranno raccolti in un pool. Nelle celle è presente solo un semplice indice di riferimento."
type: docs
url: /it/net/aspose.cells/workbook/getstyleinpool/
---
## Workbook.GetStyleInPool method

Ottiene lo stile nel pool di stili. Tutti gli stili nella cartella di lavoro saranno raccolti in un pool. Nelle celle è presente solo un semplice indice di riferimento.

```csharp
public Style GetStyleInPool(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice. |

### Valore di ritorno

Lo stile nel pool corrisponde all'indice fornito, può essere nullo.

### Osservazioni

Se lo stile restituito viene modificato, lo stile di tutte le celle (che fanno riferimento a questo stile) verrà modificato.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetStyleInPoolWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi alcuni dati di esempio
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123.45);
            ws.Cells["A3"].PutValue(DateTime.Now);
            
            // Applica alcuni stili
            Style style1 = wb.CreateStyle();
            style1.Custom = "$#,##0.00";
            ws.Cells["A2"].SetStyle(style1);
            
            Style style2 = wb.CreateStyle();
            style2.Custom = "yyyy-mm-dd";
            ws.Cells["A3"].SetStyle(style2);
            
            // Salva su stream di memoria
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                
                // Ricarica il workbook dallo stream
                ms.Position = 0;
                Workbook reloadWb = new Workbook(ms);
                
                // Ottieni e visualizza gli stili dal pool di stili
                int count = reloadWb.CountOfStylesInPool;
                Console.WriteLine($"Styles in pool: {count}");
                
                for (int i = 0; i < count; i++)
                {
                    Style style = reloadWb.GetStyleInPool(i);
                    Console.WriteLine($"Style {i}: CustomFormat={style.Custom}");
                }
            }
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


