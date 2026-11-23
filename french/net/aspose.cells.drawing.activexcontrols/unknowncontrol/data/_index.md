---
title: "UnknownControl.Data"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété UnknownControl. Obtient et définit les données binaires du contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/unknowncontrol/data/
---
## UnknownControl.Data property

Obtient et définit les données binaires du contrôle.

```csharp
public override byte[] Data { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class UnknownControlPropertyDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un CLSID factice (identifiant invalide)
            byte[] dummyClsid = new byte[16];

            // Ajouter un contrôle ActiveX inconnu en utilisant ControlType.Unknown avec tous les paramètres
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Unknown, 0, 0, 100, 100, 0, 0);

            // Accéder à l'instance UnknownControl
            UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;

            // Définir les données du contrôle, y compris le CLSID, en copiant dans le tableau existant
            Array.Copy(dummyClsid, unknownControl.Data, dummyClsid.Length);

            // Lire et afficher les informations de la propriété Data
            Console.WriteLine($"Unknown control data length: {unknownControl.Data.Length}");
            Console.WriteLine($"Control type: {unknownControl.Type}");

            // Démontrer la persistance des données de contrôle dans le fichier de sortie
            workbook.Save("UnknownControlDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


