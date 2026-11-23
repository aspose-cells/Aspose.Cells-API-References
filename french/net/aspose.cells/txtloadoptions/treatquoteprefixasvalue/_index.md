---
title: "TxtLoadOptions.TreatQuotePrefixAsValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TxtLoadOptions. Indique si le signe de guillemet simple initial doit être considéré comme faisant partie de la valeur d'une cellule. La valeur par défaut est vrai. Si elle est fausse, le guillemet simple initial sera supprimé de la valeur de la cellule correspondante et QuotePrefix sera défini sur vrai pour la cellule."
type: docs
url: /fr/net/aspose.cells/txtloadoptions/treatquoteprefixasvalue/
---
## TxtLoadOptions.TreatQuotePrefixAsValue property

Indique si le signe de guillemet simple initial doit être considéré comme faisant partie de la valeur d'une cellule. La valeur par défaut est vrai. Si elle est fausse, le guillemet simple initial sera supprimé de la valeur de la cellule correspondante et [`QuotePrefix`](../../style/quoteprefix/) sera défini sur vrai pour la cellule.

```csharp
public bool TreatQuotePrefixAsValue { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyTreatQuotePrefixAsValueDemo
    {
        public static void Run()
        {
            // Créer des données CSV d'exemple avec des préfixes de guillemets
            string csvData = "ID,Name,Value\n1,\"'Apple\",100\n2,\"'Orange\",200";
            string filePath = "test.csv";

            // Enregistrer les données CSV dans un fichier
            File.WriteAllText(filePath, csvData);

            // Scénario 1 : TreatQuotePrefixAsValue = false (par défaut)
            var loadOptions1 = new TxtLoadOptions();
            loadOptions1.TreatQuotePrefixAsValue = false;
            
            var workbook1 = new Workbook(filePath, loadOptions1);
            var worksheet1 = workbook1.Worksheets[0];
            Console.WriteLine("TreatQuotePrefixAsValue = false:");
            Console.WriteLine("Cell B2 value: " + worksheet1.Cells["B2"].Value); // Will show 'Apple (quote treated as formatting)

            // Scénario 2 : TreatQuotePrefixAsValue = true
            var loadOptions2 = new TxtLoadOptions();
            loadOptions2.TreatQuotePrefixAsValue = true;
            
            var workbook2 = new Workbook(filePath, loadOptions2);
            var worksheet2 = workbook2.Worksheets[0];
            Console.WriteLine("\nTreatQuotePrefixAsValue = true:");
            Console.WriteLine("Cell B2 value: " + worksheet2.Cells["B2"].Value); // Will show 'Apple (quote treated as value)

            // Nettoyer
            File.Delete(filePath);
        }
    }
}
```

### Voir aussi

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


