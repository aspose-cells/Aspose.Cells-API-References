---
title: "ActiveXControlBase.Workbook"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ActiveXControlBase. Obtient l'objet Workbook"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/
---
## ActiveXControlBase.Workbook property

Obtient l'objet `Workbook`.

```csharp
public Workbook Workbook { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlBasePropertyWorkbookDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter un contrôle ActiveX à la feuille de calcul
                Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 30);
                CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

                // Définir certaines propriétés pour rendre l'exemple significatif
                checkBox.Caption = "Sample CheckBox";
                checkBox.IsAutoSize = true;

                // Démontrer la propriété Workbook (lecture seule)
                Workbook controlWorkbook = checkBox.Workbook;
                Console.WriteLine("ActiveX Control Workbook reference obtained successfully.");
                Console.WriteLine("Workbook has " + controlWorkbook.Worksheets.Count + " worksheets.");

                // Vérifier que la référence du workbook est la même que notre workbook original
                if (controlWorkbook == workbook)
                {
                    Console.WriteLine("The ActiveX control's Workbook property correctly references the parent workbook.");
                }

                // Enregistrez le classeur
                workbook.Save("ActiveXControlWorkbookDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Workbook](../../../aspose.cells/workbook/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


