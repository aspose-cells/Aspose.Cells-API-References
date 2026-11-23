---
title: "AbstractLowCodeLoadOptionsProvider.Finish"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractLowCodeLoadOptionsProvider. Libère les ressources après le traitement de la partie actuelle de l'entrée"
type: docs
url: /fr/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/
---
## AbstractLowCodeLoadOptionsProvider.Finish method

Libère les ressources après le traitement de la partie actuelle de l'entrée.

```csharp
public virtual void Finish(LowCodeLoadOptions part)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| partie | LowCodeLoadOptions | les options de chargement utilisées pour la partie actuellement découpée. |

### Remarques

Par défaut, cette méthode ferme simplement le flux spécifié par le [`InputStream`](../../lowcodeloadoptions/inputstream/) directement (si les options de chargement ont spécifié un Stream comme source). L'utilisateur peut remplacer cette méthode pour contrôler la façon de libérer les ressources selon ses exigences et l'implémentation de [`Current`](../current/).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.Collections;

    public class AbstractLowCodeLoadOptionsProviderMethodFinishWithLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };

            CustomLoadOptionsProvider provider = new CustomLoadOptionsProvider(files);

            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.OutputFile = "result.xlsx";
            saveOptions.SaveFormat = SaveFormat.Xlsx;

            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            mergeOptions.LoadOptionsProvider = provider;
            mergeOptions.SaveOptions = saveOptions;

            SpreadsheetMerger.Process(mergeOptions);
        }
    }

    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {       

        public IEnumerator fileIter;
        public CustomLoadOptionsProvider(string[] files)
        {
            fileIter = files.GetEnumerator();
            current = new LowCodeLoadOptions();
        }
        private LowCodeLoadOptions current;

        public override LowCodeLoadOptions Current => current;

        public override bool MoveNext()
        {
            if (fileIter.MoveNext())
            {
                current = new LowCodeLoadOptions();
                current.InputFile = fileIter.Current.ToString();
                return true;
            }
            
            return false;
        }

        public override void Finish(LowCodeLoadOptions part)
        {
            base.Finish(part);
        }
    }
}
```

### Voir aussi

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


