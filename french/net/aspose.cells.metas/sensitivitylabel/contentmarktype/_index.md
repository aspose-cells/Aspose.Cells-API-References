---
title: "SensitivityLabel.ContentMarkType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SensitivityLabel. Obtient et définit les types de marquage de contenu qui doivent être appliqués à un fichier"
type: docs
url: /fr/net/aspose.cells.metas/sensitivitylabel/contentmarktype/
---
## SensitivityLabel.ContentMarkType property

Obtient et définit les types de marquage de contenu qui doivent être appliqués à un fichier.

```csharp
public SensitivityLabelMarkType ContentMarkType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyContentMarkTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Créez une instance de SensitivityLabel
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Définir les propriétés de base
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                
                // Démontrer la propriété ContentMarkType (lecture‑écriture)
                Console.WriteLine("Initial ContentMarkType: " + label.ContentMarkType);
                
                // Définissez différents types de marquage de contenu
                label.ContentMarkType = SensitivityLabelMarkType.Header;
                Console.WriteLine("After setting Header: " + label.ContentMarkType);
                
                label.ContentMarkType = SensitivityLabelMarkType.Watermark;
                Console.WriteLine("After setting Watermark: " + label.ContentMarkType);
                
                // Afficher l'utilisation de drapeaux combinés
                label.ContentMarkType = SensitivityLabelMarkType.Header | SensitivityLabelMarkType.Footer;
                Console.WriteLine("Combined Header+Footer: " + label.ContentMarkType);
                
                // Enregistrez le classeur
                workbook.Save("ContentMarkTypeDemo.xlsx");
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

* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


