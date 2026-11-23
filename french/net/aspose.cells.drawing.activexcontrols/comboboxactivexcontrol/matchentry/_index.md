---
title: "ComboBoxActiveXControl.MatchEntry"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ComboBoxActiveXControl. Indique comment une ListBox ou un ComboBox recherche dans sa liste pendant que l'utilisateur saisit"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/matchentry/
---
## ComboBoxActiveXControl.MatchEntry property

Indique comment une ListBox ou une ComboBox recherche dans sa liste pendant que l'utilisateur saisit.

```csharp
public ControlMatchEntryType MatchEntry { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyMatchEntryDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un contrôle ActiveX ComboBox à la feuille de calcul
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                1, 0, 1, 0, 100, 20);
            
            // Obtenir le contrôle ComboBox ActiveX
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Configurer les propriétés de base
            comboBox.Font.Name = "Arial";
            comboBox.Font.Size = 10;
            comboBox.ListRows = 8;

            // Démontrer la propriété MatchEntry
            comboBox.MatchEntry = ControlMatchEntryType.Complete; // Search as user types
            Console.WriteLine("MatchEntry set to: " + comboBox.MatchEntry);

            // Modifier MatchEntry vers un autre mode
            comboBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Search by first letter
            Console.WriteLine("MatchEntry changed to: " + comboBox.MatchEntry);

            // Enregistrez le classeur
            workbook.Save("ComboBoxActiveXControlDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* enum [ControlMatchEntryType](../../controlmatchentrytype/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


