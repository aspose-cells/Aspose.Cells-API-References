---
title: "PivotField.ShowValuesAs"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotField. Affiche les valeurs du champ de données sous un format d'affichage différent lorsque le calcul ShowDataAs est utilisé"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/showvaluesas/
---
## ShowValuesAs(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) {#showvaluesas}

Affiche les valeurs du champ de données sous un format d'affichage différent lorsque le calcul ShowDataAs est utilisé.

```csharp
[Obsolete("Use PivotField.ShowValuesAs(PivotShowValuesAsType,int int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ShowValuesAs(PivotFieldDataDisplayFormat displayFormat, int baseField, 
    PivotItemPositionType baseItemPositionType, int baseItem)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| displayFormat | PivotFieldDataDisplayFormat | Le type de format d'affichage des données. |
| baseField | Int32 | L'index du champ sur lequel se base le calcul ShowDataAs. |
| baseItemPositionType | PivotItemPositionType | Le type de position de l'élément de base. |
| baseItem | Int32 | L'index de l'élément de base sur lequel se base le calcul ShowDataAs. Fonctionne uniquement lorsque baseItemPositionType est personnalisé. |

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.ShowValuesAs(PivotShowValuesAsType,int,int). Cette méthode sera supprimée 12 mois plus tard, à compter de novembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodShowValuesAsWithPivotFieldDataDisplayFormatIntDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[workbook.Worksheets.Add()];
            worksheet.Name = "PivotData";

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Quarter");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue(1000);
            
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue(1500);
            
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue("Q1");
            worksheet.Cells["C4"].PutValue(800);
            
            worksheet.Cells["A5"].PutValue("Furniture");
            worksheet.Cells["B5"].PutValue("Q2");
            worksheet.Cells["C5"].PutValue(1200);

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Ajouter le champ de ligne
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];

            // Ajouter un champ de colonne
            int columnFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            PivotField columnField = pivotTable.ColumnFields[columnFieldIndex];

            // Ajouter un champ de données et configurer ShowValuesAs
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            dataField.DisplayName = "Sales Diff";
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, columnField.BaseIndex, PivotItemPositionType.Next, 0);

            // Calculez les données et enregistrez
            pivotTable.CalculateData();
            workbook.Save("PivotTableShowValuesAsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, int, int) {#showvaluesas_1}

Définit le calcul "Show Values As" pour ce champ de tableau croisé dynamique.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, int baseField, int baseItem)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | Type du calcul "Show Values As". |
| baseField | Int32 | Index du champ de base utilisé pour le calcul. |
| baseItem | Int32 | Index de l'élément de base pour le calcul. Utilisez [`PreviousPivotItem`](../../pivotshowvaluessetting/previouspivotitem/) (-1) pour l'élément précédent, [`NextPivotItem`](../../pivotshowvaluessetting/nextpivotitem/) (-2) pour l'élément suivant ; les valeurs non négatives désignent l'index ordinal d'un élément pivot spécifique. |

### Remarques

Uniquement pour le champ de données.

### Voir aussi

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, string, string) {#showvaluesas_2}

Configure le calcul "Show Values As" pour ce champ de données.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, string baseField, string baseItem)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | Le type de calcul pour Show Values As. |
| baseField | String | Le nom du champ de base utilisé dans le calcul. |
| baseItem | String | Légende d'un élément pivot standard. Accepte également les mots‑clés littéraux réservés : `(previous)` pour l'élément précédent, `(next)` pour l'élément suivant. Passez `null` si le type de calcul sélectionné ne nécessite pas d'élément de base. |

### Voir aussi

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


