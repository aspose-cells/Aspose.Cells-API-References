---
title: "LoadFilter.SheetsInLoadingOrder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "LoadFilter property. Spécifie les indices des feuilles et l'ordre de chargement. La valeur par défaut est null, ce qui indique de charger toutes les feuilles dans l'ordre par défaut du fichier modèle. Si ce n'est pas null et qu'un indice de feuille n'est pas présent dans le tableau retourné, alors la feuille ne sera pas chargée"
type: docs
url: /fr/net/aspose.cells/loadfilter/sheetsinloadingorder/
---
## LoadFilter.SheetsInLoadingOrder property

Spécifie les feuilles (indices) et l'ordre à charger. La valeur par défaut est null, ce qui indique de charger toutes les feuilles dans l'ordre par défaut du fichier modèle. Si la valeur n'est pas null et que l'indice d'une feuille n'est pas présent dans le tableau retourné, alors la feuille ne sera pas chargée.

```csharp
public virtual int[] SheetsInLoadingOrder { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterPropertySheetsInLoadingOrderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec plusieurs feuilles
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Créer un filtre de chargement personnalisé
            LoadFilter loadFilter = new LoadFilter(LoadDataFilterOptions.All);
            
            // Afficher le SheetsInLoadingOrder par défaut (null signifie charger toutes les feuilles)
            Console.WriteLine("Initial SheetsInLoadingOrder is null: " + (loadFilter.SheetsInLoadingOrder == null));
            
            // Créer un fichier modèle pour démontrer le chargement avec un ordre de feuilles personnalisé
            workbook.Save("Template.xlsx");
            
            // Créer des options de chargement avec notre filtre personnalisé
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = loadFilter;
            
            // Charger le classeur avec les paramètres par défaut (toutes les feuilles)
            Workbook loadedWorkbook1 = new Workbook("Template.xlsx", loadOptions);
            Console.WriteLine("Sheets loaded with default filter: " + loadedWorkbook1.Worksheets.Count);
            
            // Créer un nouveau filtre avec un ordre de chargement de feuilles spécifique
            LoadFilter orderedFilter = new LoadFilter(LoadDataFilterOptions.All)
            {
                // Remarque : SheetsInLoadingOrder est en lecture seule, nous devons donc créer un nouveau filtre
                // avec l'ordre souhaité dans le constructeur ou par d'autres moyens
                // Cela démontre la limitation de la propriété étant en lecture seule
            };
            
            // Étant donné que SheetsInLoadingOrder est en lecture seule, nous devrons sous‑classer LoadFilter
            // pour démontrer un ordre de chargement de feuilles personnalisé
            CustomLoadFilter customFilter = new CustomLoadFilter(new int[] { 2, 0 }); // Load Sheet3 first, then Sheet1
            
            LoadOptions customLoadOptions = new LoadOptions();
            customLoadOptions.LoadFilter = customFilter;
            
            // Charger le classeur avec un ordre de feuilles personnalisé
            Workbook loadedWorkbook2 = new Workbook("Template.xlsx", customLoadOptions);
            Console.WriteLine("Sheets loaded with custom filter: " + loadedWorkbook2.Worksheets.Count);
            Console.WriteLine("First sheet in custom order: " + loadedWorkbook2.Worksheets[0].Name);
        }
    }

    // Implémentation personnalisée de LoadFilter pour démontrer la fonctionnalité de SheetsInLoadingOrder
    public class CustomLoadFilter : LoadFilter
    {
        private readonly int[] _sheetsOrder;
        
        public CustomLoadFilter(int[] sheetsOrder) : base(LoadDataFilterOptions.All)
        {
            _sheetsOrder = sheetsOrder;
        }
        
        public override int[] SheetsInLoadingOrder => _sheetsOrder;
    }
}
```

### Voir aussi

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


