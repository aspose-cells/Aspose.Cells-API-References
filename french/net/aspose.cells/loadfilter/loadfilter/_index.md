---
title: "LoadFilter.LoadFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur LoadFilter. Construit un LoadFilter avec les options de filtre par défaut LoadDataFilterOptions.All"
type: docs
url: /fr/net/aspose.cells/loadfilter/loadfilter/
---
## LoadFilter() {#constructor}

Construit un LoadFilter avec les options de filtre par défaut LoadDataFilterOptions.All.

```csharp
public LoadFilter()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadFilterMethodCtorDemo
    {
        public static void Run()
        {
            // Créer un nouveau LoadFilter avec le constructeur par défaut
            LoadFilter filter = new LoadFilter();
            
            // Créer des options de chargement et assigner le filtre
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = filter;
            
            // Charger le classeur avec le filtre
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);
            
            // Démontrer l'utilisation en comptant les feuilles de calcul
            Console.WriteLine("Number of worksheets loaded: " + workbook.Worksheets.Count);
            
            // Afficher les données de cellules filtrées (toutes les cellules chargées par défaut)
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine($"Worksheet '{sheet.Name}' has {sheet.Cells.Count} cells");
            }
        }
    }
}
```

### Voir aussi

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadFilter(LoadDataFilterOptions) {#constructor_1}

Construit un LoadFilter avec les options de filtre fournies.

```csharp
public LoadFilter(LoadDataFilterOptions opts)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| opts | LoadDataFilterOptions | les options de filtre par défaut |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodCtorWithLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparer les données pour les paramètres de la méthode (LoadDataFilterOptions)
            LoadDataFilterOptions filterOptions = LoadDataFilterOptions.CellData | LoadDataFilterOptions.Chart;

            try
            {
                // Appeler la méthode #ctor avec les types de paramètres spécifiques
                LoadFilter loadFilter = new LoadFilter(filterOptions);

                // Traiter ou afficher le résultat
                Console.WriteLine("LoadFilter created successfully with LoadDataFilterOptions: " + filterOptions);

                // Afficher l'effet de l'appel de la méthode
                Console.WriteLine("LoadDataFilterOptions set to: " + loadFilter.LoadDataFilterOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LoadFilter: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("LoadFilterCtorWithLoadDataFilterOptionsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


