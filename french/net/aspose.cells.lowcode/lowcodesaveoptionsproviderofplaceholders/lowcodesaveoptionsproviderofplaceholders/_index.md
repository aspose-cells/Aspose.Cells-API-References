---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur LowCodeSaveOptionsProviderOfPlaceHolders. Instancie un objet pour fournir des options d'enregistrement selon les modèles spécifiés"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders constructor

Instancie une instance pour fournir des options d’enregistrement selon les modèles spécifiés.

```csharp
public LowCodeSaveOptionsProviderOfPlaceHolders(string pathTemplate)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pathTemplate | String | Le modèle du chemin de fichier résultant. |

### Remarques

Les espaces réservés pris en charge dans le modèle de chemin de fichier: ${SheetIndex}: sera remplacé par l'index de la feuille de la partie découpée${SheetName}: sera remplacé par le nom de la feuille de la partie découpée${SplitPartIndex}: sera remplacé par l'index de la partie découpée${SheetIndexPrefix}: sera remplacé par [`SheetIndexPrefix`](../sheetindexprefix/)${SheetNamePrefix}: sera remplacé par [`SheetNamePrefix`](../sheetnameprefix/)${SplitPartPrefix}: sera remplacé par [`SplitPartPrefix`](../splitpartprefix/)

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersMethodCtorWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Appeler la méthode #ctor avec le paramètre String
                string pathTemplate = "output_{sheet}_part_{part}.xlsx";
                var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

                // Définir certaines propriétés
                provider.SheetIndexOffset = 0;
                provider.SplitPartIndexOffset = 0;
                provider.SheetNamePrefix = "Sheet_";
                provider.SplitPartPrefix = "Part_";

                Console.WriteLine("LowCodeSaveOptionsProviderOfPlaceHolders created successfully with path template: " + pathTemplate);
                Console.WriteLine($"SheetNamePrefix: {provider.SheetNamePrefix}, SplitPartPrefix: {provider.SplitPartPrefix}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LowCodeSaveOptionsProviderOfPlaceHolders: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("LowCodeSaveOptionsProviderDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


