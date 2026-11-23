---
title: "AbstractLowCodeSaveOptionsProvider.Finish"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractLowCodeSaveOptionsProvider. Libère les ressources après le traitement de la partie actuellement scindée"
type: docs
url: /fr/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/
---
## AbstractLowCodeSaveOptionsProvider.Finish method

Libère les ressources après le traitement de la partie découpée actuelle.

```csharp
public virtual void Finish(LowCodeSaveOptions part)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| partie | LowCodeSaveOptions | les options d'enregistrement utilisées pour la partie actuellement divisée. |

### Remarques

Par défaut, cette méthode ferme simplement le flux spécifié par le [`OutputStream`](../../lowcodesaveoptions/outputstream/) directement (si les options d'enregistrement spécifient un Stream comme destination). L'utilisateur peut remplacer cette méthode pour contrôler la façon de libérer les ressources selon ses exigences et l'implémentation de [`GetSaveOptions`](../getsaveoptions/).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo
    {
        public static void Run()
        {

            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "split.xlsx";

            // Créez une instance concrète du fournisseur
            var provider = new CustomLowCodeSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
                     
          
        }
    }

    // Implémentation concrète de AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        { 
            base.Finish(part);
        }
        // Implémentez la méthode abstraite requise
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


