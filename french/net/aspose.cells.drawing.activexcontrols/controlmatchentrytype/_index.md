---
title: "Énumération ControlMatchEntryType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.ActiveXControls.ControlMatchEntryType. Représente la façon dont un ListBox ou ComboBox recherche dans sa liste pendant que l'utilisateur tape"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/controlmatchentrytype/
---
## ControlMatchEntryType enumeration

Représente la façon dont une ListBox ou une ComboBox recherche dans sa liste pendant que l'utilisateur saisit.

```csharp
public enum ControlMatchEntryType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| FirstLetter | `0` | Le contrôle recherche la prochaine entrée qui commence par le caractère saisi. Taper à plusieurs reprises la même lettre fait défiler toutes les entrées commençant par cette lettre. |
| Complete | `1` | À chaque caractère tapé, le contrôle recherche une entrée correspondant à tous les caractères saisis. |
| None | `2` | La liste ne sera pas recherchée lorsque des caractères sont tapés. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ControlMatchEntryTypeDemo
    {
        public static void ControlMatchEntryTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Ajoutez un contrôle ActiveX ComboBox à la feuille de calcul
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Définissez les propriétés de la ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 3;
            comboBox.ColumnCount = 1;
            comboBox.MatchEntry = ControlMatchEntryType.Complete; // Set the MatchEntry type to Complete
            comboBox.IsEditable = true;

            // Ajouter des éléments à la ComboBox
            comboBox.Value = "Apple;Banana;Cherry";

            // Ajouter un contrôle ActiveX ListBox à la feuille de calcul
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;

            // Définir les propriétés du ListBox
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Set the MatchEntry type to FirstLetter
            listBox.SelectionType = SelectionType.Single;

            // Ajouter des éléments au ListBox
            listBox.Value = "Apple;Banana;Cherry";

            // Enregistrez le classeur
            workbook.Save("ControlMatchEntryTypeExample.xlsx");
            workbook.Save("ControlMatchEntryTypeExample.pdf");

            // Afficher les résultats
            Console.WriteLine("ComboBox and ListBox with different MatchEntry types have been created and saved to ControlMatchEntryTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


