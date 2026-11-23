---
title: "PivotField.GroupBy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotField. Regroupe automatiquement le champ avec un intervalle"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/groupby/
---
## GroupBy(double, bool) {#groupby_7}

Regroupez automatiquement le champ avec un intervalle

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(double interval, bool newField)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| intervalle | Double | L'interne du groupe. Une valeur automatique sera assignée si elle est zéro, |
| newField | Boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique est autorisé. Seulement pour le groupe DateTime. |

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions). Cette méthode sera supprimée dans 6 mois, à partir de septembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder au premier tableau croisé dynamique
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Ajouter le champ à la zone de colonnes
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 2);
            
            // Regroupez le champ par 1 (intervalle) avec une plage automatique
            pivotTable.BaseFields[2].GroupBy(1.0, true);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(PivotGroupByType[], double, bool) {#groupby_6}

Regroupez automatiquement le champ avec interne

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(PivotGroupByType[] groups, double interval, bool newField)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| groupes | PivotGroupByType[] | Types de groupe |
| intervalle | Double | L'interne du groupe. Une valeur automatique sera assignée si elle est zéro, ne fonctionne que pour le regroupement par Nombres ou Jours. |
| newField | Boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique est autorisé. |

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions). Cette méthode sera supprimée dans 6 mois, à partir de septembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Voir aussi

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DateTime, DateTime, PivotGroupByType[], double, bool) {#groupby_5}

Regroupez le fichier par les types de groupe de dates.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DateTime start, DateTime end, PivotGroupByType[] groups, double interval, 
    bool firstAsNewField)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| début | DateTime | La date et heure de début |
| fin | DateTime | La date et heure de fin |
| groupes | PivotGroupByType[] | Types de groupe |
| intervalle | Double | L'intervalle |
| firstAsNewField | Boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique. Seulement pour le premier élément du groupe. |

### Valeur de retour

False signifie que ce champ ne peut pas être groupé par date et heure.

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions). Cette méthode sera supprimée dans 6 mois, à partir de septembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithDateTimeDateTimePivotGroupByTyDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple avec des dates pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
            worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
            worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
            worksheet.Cells["A5"].Value = new DateTime(2023, 4, 5);
            worksheet.Cells["A6"].Value = new DateTime(2023, 5, 25);
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1500;
            worksheet.Cells["B3"].Value = 2300;
            worksheet.Cells["B4"].Value = 3200;
            worksheet.Cells["B5"].Value = 4100;
            worksheet.Cells["B6"].Value = 5000;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Obtenez le champ du tableau croisé
            PivotField pivotField = pivotTable.RowFields[0];

            // Préparez les paramètres pour la méthode GroupBy
            DateTime startDate = new DateTime(2023, 1, 1);
            DateTime endDate = new DateTime(2023, 6, 30);
            PivotGroupByType[] groupTypes = new PivotGroupByType[] { PivotGroupByType.Months };
            double interval = 1;
            bool firstAsNewField = false;

            try
            {
                // Appelez la méthode GroupBy avec des paramètres de date
                bool result = pivotField.GroupBy(startDate, endDate, groupTypes, interval, firstAsNewField);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Actualiser le tableau croisé dynamique
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("PivotFieldGroupByDateTimeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) {#groupby_3}

Regroupez le fichier par les types de groupe de dates.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, DateTime start, bool isAutoEnd, DateTime end, 
    PivotGroupByType[] groups, double interval, bool firstAsNewField)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isAutoStart | Boolean | Indique si la valeur de date et heure de début doit être détectée automatiquement. |
| début | DateTime | La date et heure de début |
| isAutoEnd | Boolean | Indique si la valeur de date et heure de fin doit être détectée automatiquement. |
| fin | DateTime | La date et heure de fin |
| groupes | PivotGroupByType[] | Types de groupe |
| intervalle | Double | L'intervalle |
| firstAsNewField | Boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique. Seulement pour le premier élément du groupe. |

### Valeur de retour

False signifie que ce champ ne peut pas être groupé par date et heure.

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions). Cette méthode sera supprimée dans 6 mois, à partir de septembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Voir aussi

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(double, double, double, bool) {#groupby_4}

Regroupez le fichier par nombre.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(double start, double end, double interval, bool newField)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| début | Double | La valeur de départ |
| fin | Double | La valeur de fin |
| intervalle | Double | L'intervalle |
| newField | Boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique |

### Valeur de retour

False signifie que ce champ ne peut pas être groupé par date et heure.

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions). Cette méthode sera supprimée dans 6 mois, à partir de septembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleDoubleDoubleBooleanDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Value";
            worksheet.Cells["A2"].Value = 1;
            worksheet.Cells["A3"].Value = 2;
            worksheet.Cells["A4"].Value = 3;
            worksheet.Cells["A5"].Value = 4;
            worksheet.Cells["A6"].Value = 5;
            worksheet.Cells["A7"].Value = 6;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:A7", "D1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Ajoutez un champ de ligne et regroupez-le
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.GroupBy(1, 6, 2, false); // Group values from 1 to 6 with interval 2, auto range false
            
            // Enregistrez le classeur
            workbook.Save("PivotGroupByExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, double, bool, double, double, bool) {#groupby_2}

Regroupez le fichier par nombre.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, double start, bool isAutoEnd, double end, double interval, 
    bool newField)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isAutoStart | Boolean | Indique si la valeur de départ doit être détectée automatiquement. |
| début | Double | La valeur de départ |
| isAutoEnd | Boolean | Indique si la valeur de fin doit être détectée automatiquement. |
| fin | Double | La valeur de fin |
| intervalle | Double | L'intervalle |
| newField | Boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique |

### Valeur de retour

False signifie que ce champ ne peut pas être groupé par date et heure.

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions). Cette méthode sera supprimée dans 6 mois, à partir de septembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(CustomPiovtFieldGroupItem[], bool) {#groupby}

Regroupez le champ de manière personnalisée.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(CustomPiovtFieldGroupItem[] customGroupItems, bool newField)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| customGroupItems | CustomPiovtFieldGroupItem[] | Les éléments de groupe personnalisés. |
| newField | Boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique |

### Valeur de retour

False signifie que ce champ ne peut pas être groupé par date et heure.

### Remarques

NOTE: Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions options) avec la propriété PivotFieldGroupOptions.DiscreteGroupItems. Cette méthode sera supprimée dans 6 mois, depuis juillet 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithCustomPiovtFieldGroupItemBooDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Grapes";
            worksheet.Cells["A6"].Value = "Mango";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            worksheet.Cells["B5"].Value = 4000;
            worksheet.Cells["B6"].Value = 5000;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Obtenez le champ du tableau croisé
            PivotField pivotField = pivotTable.RowFields[0];

            // Créer des éléments de groupe personnalisés
            CustomPiovtFieldGroupItem[] customGroupItems = new CustomPiovtFieldGroupItem[2];
            customGroupItems[0] = new CustomPiovtFieldGroupItem("Group1", new int[] { 0, 1 }); // Apple (index 0), Banana (index 1)
            customGroupItems[1] = new CustomPiovtFieldGroupItem("Group2", new int[] { 2, 3, 4 }); // Orange (2), Grapes (3), Mango (4)

            try
            {
                // Appeler la méthode GroupBy avec des éléments de groupe personnalisés
                bool result = pivotField.GroupBy(customGroupItems, false);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Actualiser le tableau croisé dynamique
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("PivotFieldGroupByCustomDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DiscreteGroupItem[], bool) {#groupby_1}

Regroupez le champ de manière personnalisée.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DiscreteGroupItem[] customGroupItems, bool newField)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| customGroupItems | DiscreteGroupItem[] | Les éléments de groupe personnalisés. |
| newField | Boolean | Indique si l'ajout d'un nouveau champ au tableau croisé dynamique |

### Remarques

NOTE: Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotField.Group(PivotFieldGroupOptions options) avec la propriété PivotFieldGroupOptions.DiscreteGroupItems. Cette méthode sera supprimée dans 6 mois, depuis juillet 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Voir aussi

* class [DiscreteGroupItem](../../discretegroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


