---
title: "WorksheetCollection.Insert"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorksheetCollection. Insérer une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/insert/
---
## Insert(int, SheetType) {#insert}

Insérer une feuille de calcul.

```csharp
public Worksheet Insert(int index, SheetType sheetType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'index de la feuille |
| sheetType | SheetType | Le type de feuille. |

### Valeur de retour

Renvoie une feuille de calcul insérée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Insert(1, SheetType.Worksheet);
            worksheet.Name = "InsertedSheet";
            workbook.Worksheets[0].Cells["A1"].Value = "Referencing inserted sheet:";
            workbook.Worksheets[0].Cells["A2"].Formula = "='InsertedSheet'!A1";
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Insert(int, SheetType, string) {#insert_1}

Insérer une feuille de calcul.

```csharp
public Worksheet Insert(int index, SheetType sheetType, string sheetName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'index de la feuille |
| sheetType | SheetType | Le type de feuille. |
| sheetName | String | Le nom de la feuille. |

### Valeur de retour

Renvoie une feuille de calcul insérée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Insérer une nouvelle feuille de calcul à l'index 0 avec le nom "InsertedSheet"
            workbook.Worksheets.Insert(0, SheetType.Worksheet, "InsertedSheet");
            
            // Accéder à la feuille de calcul insérée
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Mettre des données dans la cellule A1 de la feuille insérée
            worksheet.Cells["A1"].PutValue("This sheet was inserted using Insert method");
            
            // Enregistrez le classeur
            workbook.Save("WorksheetInsertDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


