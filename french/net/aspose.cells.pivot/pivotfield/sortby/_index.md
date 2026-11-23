---
title: "PivotField.SortBy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotField. Trie ce champ de tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/sortby/
---
## SortBy(SortOrder) {#sortby}

Trie ce champ pivot.

```csharp
public void SortBy(SortOrder sortType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sortType | SortOrder | Le type de tri de ce champ. |

### Voir aussi

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int) {#sortby_1}

Trie ce champ pivot.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method or PivotField.IsAutoSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sortType | SortOrder | Le type de tri de ce champ. |
| fieldSortedBy | Int32 | L'index du champ pivot utilisé pour le tri. -1 signifie trier par les libellés de données de ce champ, les autres valeurs indiquent l'index du champ de données utilisé pour le tri. |

### Remarques

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la méthode PivotField.SortBy(SortOrder, int,string) ou la propriété PivotField.IsAutoSort. Cette méthode sera supprimée 12 mois après, soit depuis septembre 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("UK");
            worksheet.Cells["A4"].PutValue("Germany");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Ajouter le champ de ligne
            int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            PivotField rowField = pivotTable.RowFields[rowIndex];
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Trier le champ de ligne par ordre décroissant avec l'index -1
            rowField.SortBy(SortOrder.Descending, -1);
            
            // Actualiser et calculer le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, PivotLineType, string) {#sortby_2}

Trie ce champ pivot.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy, PivotLineType dataType, string cellName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sortType | SortOrder | Le type de tri de ce champ. |
| fieldSortedBy | Int32 | L'index du champ pivot utilisé pour le tri. -1 signifie trier par les libellés de données de ce champ, les autres valeurs indiquent l'index du champ de données utilisé pour le tri. |
| dataType | PivotLineType | Le type de données triées. |
| cellName | String | Trier par valeurs dans la ligne ou la colonne |

### Remarques

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la méthode PivotField.SortBy(SortOrder, int,string). Cette méthode sera supprimée 12 mois après, soit depuis septembre 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32PivotLineTypeStrDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("B");
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);
            worksheet.Cells["B4"].PutValue(100);

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Trier le champ de ligne
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E4");
            
            // Calculer les données
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SortOrder](../../../aspose.cells/sortorder/)
* enum [PivotLineType](../../pivotlinetype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, string) {#sortby_3}

Trie ce champ pivot.

```csharp
public void SortBy(SortOrder sortType, int fieldSortedBy, string cellName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sortType | SortOrder | Le type de tri de ce champ. |
| fieldSortedBy | Int32 | L'index du champ pivot utilisé pour le tri. -1 signifie trier par les libellés de données de ce champ, les autres valeurs indiquent l'index du champ de données utilisé pour le tri. |
| cellName | String | Trier par valeurs dans la ligne ou la colonne. Si Null, regrouper par le total du champ, sinon regrouper par les valeurs de la colonne ou de la ligne sélectionnée. |

### Voir aussi

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


