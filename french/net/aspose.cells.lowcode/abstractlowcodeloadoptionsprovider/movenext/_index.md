---
title: "AbstractLowCodeLoadOptionsProvider.MoveNext"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractLowCodeLoadOptionsProvider. Vérifie s'il y a plus d'entrée"
type: docs
url: /fr/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/movenext/
---
## AbstractLowCodeLoadOptionsProvider.MoveNext method

Vérifie s'il y a plus d'entrée.

```csharp
public abstract bool MoveNext()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.Collections;

    public class AbstractLowCodeLoadOptionsProviderMethodMoveNextDemo
    {
        public static void Run()
        {
            string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };
            // Créer un fournisseur personnalisé qui implémente AbstractLowCodeLoadOptionsProvider
            MultiFileProvider provider = new MultiFileProvider(files);

            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.OutputFile = "result.xlsx";
            saveOptions.SaveFormat = SaveFormat.Xlsx;

            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            mergeOptions.LoadOptionsProvider = provider;
            mergeOptions.SaveOptions = saveOptions;

            SpreadsheetMerger.Process(mergeOptions);

        }

        private class MultiFileProvider : AbstractLowCodeLoadOptionsProvider
        {
            public IEnumerator fileIter;
            public MultiFileProvider(string[] files)
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
}
```

### Voir aussi

* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


