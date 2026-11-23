---
title: "LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode LowCodeSaveOptionsProviderOfAssembling. Obtient les options d'enregistrement à partir desquelles récupérer les paramètres de sortie pour la partie actuellement divisée"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/
---
## LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions method

Obtient les options d’enregistrement à partir desquelles récupérer les paramètres de sortie pour la partie découpée actuelle.

```csharp
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingMethodGetSaveOptionsWithSplitPartInfoDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "Sample Data for Split";

            try
            {
                // Créer une instance de LowCodeSaveOptionsProviderOfAssembling
                var provider = new LowCodeSaveOptionsProviderOfAssembling
                {
                    PathHeader = "Output/",
                    PathTail = ".xlsx",
                    UseSheetName = true,
                    SheetPrefix = "Sheet_",
                    SplitPartPrefix = "Part_",
                    SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
                };

                // Créer une instance de SplitPartInfo en utilisant la réflexion puisque le constructeur n'est pas accessible
                var splitPartInfo = (SplitPartInfo)Activator.CreateInstance(typeof(SplitPartInfo), nonPublic: true);

                // Appeler GetSaveOptions avec le paramètre SplitPartInfo
                LowCodeSaveOptions saveOptions = provider.GetSaveOptions(splitPartInfo);

                Console.WriteLine("SaveOptions created successfully");
                Console.WriteLine($"Output format: {saveOptions.SaveFormat}");

                // Enregistrer le classeur (dans une utilisation réelle, cela utiliserait les options d'enregistrement générées)
                workbook.Save("GetSaveOptionsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in GetSaveOptions demo: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


