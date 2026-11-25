---
title: "CheckBoxCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CheckBoxCollection. Restituisce l'elemento CheckBox all'indice specificato"
type: docs
url: /it/net/aspose.cells.drawing/checkboxcollection/item/
---
## CheckBoxCollection indexer

Restituisce l'elemento [`CheckBox`](../../checkbox/) all'indice specificato.

```csharp
public CheckBox this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una casella di controllo al foglio di lavoro
            int index = worksheet.CheckBoxes.Add(10, 10, 100, 20);
            
            // Accedi al checkbox usando la proprietà Item (indicizzatore)
            Aspose.Cells.Drawing.CheckBox checkBox = worksheet.CheckBoxes[index];
            checkBox.Text = "Sample CheckBox";
            checkBox.Name = "CheckBox1";
            
            // Accedi al checkbox usando l'indice (proprietà Item)
            Aspose.Cells.Drawing.CheckBox checkBoxByName = worksheet.CheckBoxes[0];
            
            // Visualizza le proprietà del checkbox
            Console.WriteLine("CheckBox Name: " + checkBoxByName.Name);
            Console.WriteLine("CheckBox Text: " + checkBoxByName.Text);
            
            // Salva la cartella di lavoro
            workbook.Save("CheckBoxExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [CheckBox](../../checkbox/)
* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


