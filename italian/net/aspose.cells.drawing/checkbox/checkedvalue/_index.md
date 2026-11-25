---
title: "CheckBox.CheckedValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CheckBox. Ottiene o imposta il valore della casella di controllo"
type: docs
url: /it/net/aspose.cells.drawing/checkbox/checkedvalue/
---
## CheckBox.CheckedValue property

Ottiene o imposta il valore della casella di controllo.

```csharp
public CheckValueType CheckedValue { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxPropertyCheckedValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi una casella di controllo al foglio di lavoro
            CheckBox checkBox = sheet.Shapes.AddCheckBox(1, 1, 100, 100, 20, 20);

            // Imposta il valore della casella di controllo su Selezionato
            checkBox.CheckedValue = CheckValueType.Checked;

            // Salva la cartella di lavoro
            workbook.Save("CheckBoxCheckedValueDemo.xlsx");

            // Carica la cartella di lavoro salvata per verificare
            Workbook loadedWorkbook = new Workbook("CheckBoxCheckedValueDemo.xlsx");
            CheckBox loadedCheckBox = (CheckBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Restituisci lo stato della casella di controllo
            Console.WriteLine("CheckBox CheckedValue: " + loadedCheckBox.CheckedValue);
        }
    }
}
```

### Vedi anche

* enum [CheckValueType](../../checkvaluetype/)
* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


