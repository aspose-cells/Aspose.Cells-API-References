---
title: "Name.GetReferredAreas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Name. Ottiene tutti i riferimenti indicati da questo nome"
type: docs
url: /it/net/aspose.cells/name/getreferredareas/
---
## Name.GetReferredAreas method

Ottiene tutti i riferimenti referenziati da questo nome.

```csharp
public ReferredArea[] GetReferredAreas(bool recalculate)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ricalcola | Booleano | se ricalcolarlo se questo nome è stato calcolato prima di questa invocazione. |

### Valore di ritorno

Tutti gli intervalli.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetReferredAreasWithBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook wb = new Workbook();
            
            // Aggiungi alcuni dati al foglio di lavoro
            wb.Worksheets[0].Cells[3, 3].PutValue("v03");
            
            // Crea un intervallo denominato con più riferimenti
            Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")];
            n.RefersTo = "='C:\\[extlink1.xlsx]Sheet1'!$A$1:$B$2,'C:\\[extlink2.xlsx]Sheet2'!$C$3,Sheet1!$D$4,'C:\\[extlink1.xlsx]Sheet1'!E5";
            
            // Ottieni le aree di riferimento con collegamenti esterni
            ReferredArea[] ras = n.GetReferredAreas(true);
            
            // Visualizza le informazioni su ogni area di riferimento
            Console.WriteLine("Number of referred areas: " + ras.Length);
            for (int i = 0; i < ras.Length; i++)
            {
                ReferredArea ra = ras[i];
                Console.WriteLine($"\nArea {i + 1}:");
                Console.WriteLine($"IsExternalLink: {ra.IsExternalLink}");
                if (ra.IsExternalLink)
                {
                    Console.WriteLine($"ExternalFileName: {ra.ExternalFileName}");
                }
                Console.WriteLine($"SheetName: {ra.SheetName}");
                Console.WriteLine($"IsArea: {ra.IsArea}");
                
                if (ra.IsArea)
                {
                    Console.WriteLine($"Range: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}" +
                                    $" to {CellsHelper.CellIndexToName(ra.EndRow, ra.EndColumn)}");
                }
                else
                {
                    Console.WriteLine($"Cell: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}");
                }
            }
            
            // Crea una cartella di lavoro esterna e aggiorna i valori
            Workbook wb1 = new Workbook();
            wb1.Worksheets[0].Cells[0, 0].PutValue("v10");
            wb1.Worksheets[0].Cells[1, 1].PutValue("v11");
            wb1.Worksheets[0].Cells[4, 4].PutValue("v14");
            
            // Aggiorna la fonte dati collegata
            wb.UpdateLinkedDataSource(new Workbook[]{wb1});
            
            // Visualizza alcuni valori dalle aree di riferimento
            Console.WriteLine("\nValues from referred areas:");
            Console.WriteLine($"Area1[0,0]: {ras[0].GetValue(0, 0)}");
            Console.WriteLine($"Area1[1,1]: {ras[0].GetValue(1, 1)}");
            Console.WriteLine($"Area3[0,0]: {ras[2].GetValue(0, 0)}");
            Console.WriteLine($"Area4[0,0]: {ras[3].GetValue(0, 0)}");
        }
    }
}
```

### Vedi anche

* class [ReferredArea](../../referredarea/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


