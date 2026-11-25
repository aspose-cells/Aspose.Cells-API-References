---
title: "DxfCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DxfCollection. Ottiene l'elemento all'indice specificato"
type: docs
url: /it/net/aspose.cells/dxfcollection/item/
---
## DxfCollection indexer

Ottiene l'elemento all'indice specificato.

```csharp
public Style this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice specificato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DxfCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi al DxfCollection dal workbook
            DxfCollection dxfCollection = workbook.Worksheets.Dxfs;

            // Crea un nuovo stile (non è possibile aggiungere direttamente a DxfCollection poiché non ha un metodo Add)
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            // Lo stile viene aggiunto automaticamente alla collezione quando viene creato

            // Ottieni il primo elemento da DxfCollection usando la proprietà Item
            Style firstStyle = dxfCollection[0];
            Console.WriteLine("First style font name: " + firstStyle.Font.Name);

            // Modifica lo stile tramite la proprietà Item (poiché restituisce un riferimento)
            firstStyle.Font.Color = System.Drawing.Color.Red;
            firstStyle.Font.IsBold = true;

            // Verifica la modifica
            Console.WriteLine("Modified style font color: " + dxfCollection[0].Font.Color);
            Console.WriteLine("Modified style font bold: " + dxfCollection[0].Font.IsBold);

            // Applica lo stile a una cella per vedere l'effetto
            worksheet.Cells["A1"].PutValue("DxfCollection Property Item Demo");
            worksheet.Cells["A1"].SetStyle(dxfCollection[0]);

            // Salva il risultato
            workbook.Save("DxfCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [DxfCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


