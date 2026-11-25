---
title: "ShapeCollection.AddComboBox"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge un ComboBox al foglio di lavoro"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addcombobox/
---
## ShapeCollection.AddComboBox method

Aggiunge un ComboBox al foglio di lavoro.

```csharp
public ComboBox AddComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale del ComboBox dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale del ComboBox dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza del ComboBox, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza del ComboBox, in unità di pixel. |

### Valore di ritorno

Un oggetto ComboBox.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddComboBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni la collezione di forme
            ShapeCollection shapes = worksheet.Shapes;

            // Aggiungi un combo box con i parametri specificati
            Aspose.Cells.Drawing.ComboBox comboBox = shapes.AddComboBox(1, 0, 1, 0, 100, 50);

            // Aggiungi elementi al combo box impostando i valori delle celle
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Imposta l'intervallo di input per la casella combinata
            comboBox.InputRange = "A1:A3";
            comboBox.DropDownLines = 3;

            // Salva la cartella di lavoro
            workbook.Save("AddComboBoxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ComboBox](../../combobox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


