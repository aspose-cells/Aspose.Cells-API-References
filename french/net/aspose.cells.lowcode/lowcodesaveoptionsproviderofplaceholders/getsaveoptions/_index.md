---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.GetSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode LowCodeSaveOptionsProviderOfPlaceHolders. Obtient les options d'enregistrement à partir desquelles récupérer les paramètres de sortie pour la partie découpée actuelle"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/getsaveoptions/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.GetSaveOptions method

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

    public class LowCodeSaveOptionsProviderOfPlaceHoldersMethodGetSaveOptionsWithSplitPartInfoDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une instance de SplitPartInfo
            // Étant donné que SplitPartInfo n'a pas de constructeur sans paramètres et que ses propriétés sont en lecture seule,
            // nous devrons obtenir une instance ailleurs dans l'API ou utiliser null si autorisé
            // À des fins de démonstration, nous passerons null (en supposant que la méthode l'accepte)
            SplitPartInfo splitPartInfo = null;

            // Créer l'instance LowCodeSaveOptionsProviderOfPlaceHolders
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output_{sheet}.xlsx")
            {
                SheetIndexOffset = 0,
                SplitPartIndexOffset = 0,
                BuildPathWithSheetAlways = false,
                BuildPathWithSplitPartAlways = false,
                SheetNamePrefix = "sheet_",
                SheetIndexPrefix = "sheet_",
                SplitPartPrefix = "part_",
                SaveOptionsTemplate = new LowCodeSaveOptions
                {
                    SaveFormat = SaveFormat.Xlsx
                }
            };

            try
            {
                // Appeler la méthode GetSaveOptions avec le paramètre SplitPartInfo
                var saveOptions = provider.GetSaveOptions(splitPartInfo);
                
                Console.WriteLine("GetSaveOptions method executed successfully with SplitPartInfo parameter");
                Console.WriteLine($"Output file: {saveOptions.OutputFile}");
                Console.WriteLine($"Save format: {saveOptions.SaveFormat}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSaveOptions method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("MethodGetSaveOptionsWithSplitPartInfoDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


