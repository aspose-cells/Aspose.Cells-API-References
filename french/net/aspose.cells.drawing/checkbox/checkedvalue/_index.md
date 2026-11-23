---
title: "CheckBox.CheckedValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CheckBox. Obtient ou définit la valeur de la case à cocher"
type: docs
url: /fr/net/aspose.cells.drawing/checkbox/checkedvalue/
---
## CheckBox.CheckedValue property

Obtient ou définit la valeur de la case à cocher.

```csharp
public CheckValueType CheckedValue { get; set; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter une case à cocher à la feuille de calcul
            CheckBox checkBox = sheet.Shapes.AddCheckBox(1, 1, 100, 100, 20, 20);

            // Définir la valeur de la case à cocher sur Coché
            checkBox.CheckedValue = CheckValueType.Checked;

            // Enregistrez le classeur
            workbook.Save("CheckBoxCheckedValueDemo.xlsx");

            // Chargez le classeur enregistré pour vérifier
            Workbook loadedWorkbook = new Workbook("CheckBoxCheckedValueDemo.xlsx");
            CheckBox loadedCheckBox = (CheckBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Afficher l'état de la case à cocher
            Console.WriteLine("CheckBox CheckedValue: " + loadedCheckBox.CheckedValue);
        }
    }
}
```

### Voir aussi

* enum [CheckValueType](../../checkvaluetype/)
* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


