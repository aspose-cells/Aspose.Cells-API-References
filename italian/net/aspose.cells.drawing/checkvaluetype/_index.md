---
title: "Enum CheckValueType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.CheckValueType. Rappresenta il tipo di valore di controllo della casella di spunta"
type: docs
url: /it/net/aspose.cells.drawing/checkvaluetype/
---
## CheckValueType enumeration

Rappresenta il tipo di valore di controllo della casella di controllo.

```csharp
public enum CheckValueType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| UnChecked | `0` | UnChecked |
| Checked | `1` | Checked |
| Mixed | `2` | Mixed |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassCheckValueTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi caselle di controllo al foglio di lavoro
            int checkboxIndex1 = sheet.CheckBoxes.Add(0, 0, 100, 100);
            int checkboxIndex2 = sheet.CheckBoxes.Add(0, 1, 100, 100);

            // Ottieni le caselle di controllo e imposta le loro proprietà
            Aspose.Cells.Drawing.CheckBox checkbox1 = sheet.CheckBoxes[checkboxIndex1];
            Aspose.Cells.Drawing.CheckBox checkbox2 = sheet.CheckBoxes[checkboxIndex2];

            // Imposta i valori delle caselle di controllo e lo stato selezionato
            checkbox1.Value = true;
            checkbox1.CheckedValue = CheckValueType.Checked;
            
            checkbox2.Value = false;
            checkbox2.CheckedValue = CheckValueType.UnChecked;  // Note: Changed from Unchecked to UnChecked

            // Collega le caselle di controllo alle celle
            checkbox1.LinkedCell = "A1";
            checkbox2.LinkedCell = "A2";

            // Genera l'output dei valori delle celle per dimostrare il collegamento
            Console.WriteLine("Cell A1 value (should be true): " + sheet.Cells["A1"].BoolValue);
            Console.WriteLine("Cell A2 value (should be false): " + sheet.Cells["A2"].BoolValue);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


