---
title: "WorkbookDesigner.GetSmartMarkers"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorkbookDesigner. Restituisce una collezione di smart marker in un foglio elettronico"
type: docs
url: /it/net/aspose.cells/workbookdesigner/getsmartmarkers/
---
## WorkbookDesigner.GetSmartMarkers method

Restituisce una raccolta di smart marker in un foglio di calcolo.

```csharp
public string[] GetSmartMarkers()
```

### Valore di ritorno

Una collezione di smart marker

### Osservazioni

Un array di stringhe viene creato ad ogni chiamata. L'array è ordinato e i valori duplicati vengono rimossi.

### Esempi

```csharp
using System;
using System.Data;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodGetSmartMarkersDemo
    {
        public static void Run()
        {
            // Crea un file modello di esempio in memoria
            Workbook templateWorkbook = new Workbook();
            Cells cells = templateWorkbook.Worksheets[0].Cells;
            
            // Aggiungi smart marker al modello
            cells["A1"].PutValue("&=COLORS_TIMES.COLORS");
            cells["B1"].PutValue("&=COLORS_TIMES.TIMES");
            
            // Salva il modello nello stream di memoria
            MemoryStream templateStream = new MemoryStream();
            templateWorkbook.Save(templateStream, SaveFormat.Xlsx);
            
            // Inizializza WorkbookDesigner con il modello
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook(templateStream);
            
            // Recupera e visualizza i marker intelligenti
            string[] smartMarkers = designer.GetSmartMarkers();
            Console.WriteLine("Found smart markers:");
            foreach (string marker in smartMarkers)
            {
                Console.WriteLine(marker);
            }
            
            // Prepara la fonte dati
            DataTable data = new DataTable("COLORS_TIMES");
            data.Columns.Add("COLORS", typeof(string));
            data.Columns.Add("TIMES", typeof(DateTime));
            data.Rows.Add("red", DateTime.Now.AddDays(-1));
            data.Rows.Add("yellow", DateTime.Now);
            data.Rows.Add("green", DateTime.Now.AddDays(1));
            
            // Imposta la fonte dati ed elabora
            designer.SetDataSource(data);
            designer.Process();
            
            // Salva il risultato
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


