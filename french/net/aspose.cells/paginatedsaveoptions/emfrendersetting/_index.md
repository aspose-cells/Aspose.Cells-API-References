---
title: "PaginatedSaveOptions.EmfRenderSetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaginatedSaveOptions. Paramètre pour le rendu du métafichier Emf"
type: docs
url: /fr/net/aspose.cells/paginatedsaveoptions/emfrendersetting/
---
## PaginatedSaveOptions.EmfRenderSetting property

Paramètre pour le rendu du métafichier Emf.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### Remarques

Les métafichiers EMF identifiés comme "EMF+ Dual" peuvent contenir à la fois des enregistrements EMF+ et des enregistrements EMF. Chaque type d'enregistrement peut être utilisé pour rendre l'image, uniquement les enregistrements EMF+, ou uniquement les enregistrements EMF. Lorsque EmfPlusPrefer est défini, les enregistrements EMF+ seront analysés lors du rendu de la page, sinon seuls les enregistrements EMF seront analysés. La valeur par défaut est EmfOnly.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());

            // Créer une image pour la démonstration EMF
            worksheet.Pictures.Add(10, 10, "example.png");

            // Configurer les options d'enregistrement avec les paramètres EMF en utilisant PdfSaveOptions
            PdfSaveOptions options = new PdfSaveOptions()
            {
                EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer
            };

            // Enregistrer le classeur avec les paramètres EMF
            workbook.Save("EmfRenderSettingDemo.pdf", options);
        }
    }
}
```

### Voir aussi

* enum [EmfRenderSetting](../../emfrendersetting/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


