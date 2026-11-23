---
title: "PivotTable.GetSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Obtient la source de données de ce tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/getsource/
---
## GetSource() {#getsource}

Obtient la source de données de ce tableau croisé dynamique.

```csharp
public string[] GetSource()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Obtenir et afficher la plage de données source
            string[] sourceData = pivotTable.GetSource();
            Console.WriteLine("Pivot Table Source: " + sourceData[0]);
            
            // Modifier la source de données
            pivotTable.ChangeDataSource(new[] { "A1:B4" });
            
            // Vérifier la source modifiée
            sourceData = pivotTable.GetSource();
            Console.WriteLine("Updated Pivot Table Source: " + sourceData[0]);
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GetSource(bool) {#getsource_1}

Obtient la source de données de ce tableau croisé dynamique.

```csharp
public string[] GetSource(bool isOriginal)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isOriginal | Boolean | Indique s'il faut renvoyer la source originale ou la source affichée. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder au premier tableau croisé dynamique
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Obtenir les données source avec le chemin local (true)
            string[] localSource = pivotTable.GetSource(true);
            Console.WriteLine("Local path source: " + localSource[0]);
            
            // Obtenir les données source avec le chemin complet (false)
            string[] fullSource = pivotTable.GetSource(false);
            Console.WriteLine("Full path source: " + fullSource[0]);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


