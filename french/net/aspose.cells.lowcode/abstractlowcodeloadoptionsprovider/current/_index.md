---
title: "AbstractLowCodeLoadOptionsProvider.Current"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AbstractLowCodeLoadOptionsProvider. Obtient les options de chargement à partir desquelles charger les données de la partie actuellement traitée"
type: docs
url: /fr/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/
---
## AbstractLowCodeLoadOptionsProvider.Current property

Obtient les options de chargement à partir desquelles charger les données de la partie actuellement traitée.

```csharp
public abstract LowCodeLoadOptions Current { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.Collections;

    public class AbstractLowCodeLoadOptionsProviderPropertyCurrentDemo
    {
        public static void Run()
        {
            string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };
            // Initialiser le fournisseur personnalisé avec nos options de chargement
            CustomProvider provider = new CustomProvider(files);
            
            int counter = 1;
            while (provider.MoveNext())
            {
                // Accéder à la propriété Current pour obtenir les options de chargement actives
                Console.WriteLine($"Processing set {counter}");
                    
                // Créer un classeur en utilisant le fichier/flux d'entrée des options de chargement actuelles
                Workbook workbook;
                if (provider.Current.InputFile != null)
                {
                    workbook = new Workbook(provider.Current.InputFile);
                }
                else if (provider.Current.InputStream != null)
                {
                    workbook = new Workbook(provider.Current.InputStream);
                }
                else
                {
                    workbook = new Workbook();
                }

                Worksheet worksheet = workbook.Worksheets[0];

                // Démontrer l'impact de l'option supprimé en raison d'une propriété manquante
                worksheet.Cells["A1"].Value = "Sample Value";

                // Enregistrer le résultat
                workbook.Save($"CurrentDemo_{counter}.xlsx");
                counter++;
            }
        }
    }

    // Implémentation d'un fournisseur personnalisé avec IDisposable
    public class CustomProvider : AbstractLowCodeLoadOptionsProvider
    {
        
        public IEnumerator fileIter;

        public CustomProvider(string[] files)
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


