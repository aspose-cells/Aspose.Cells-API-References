---
title: "Cells.InsertColumns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Insère quelques colonnes dans la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/cells/insertcolumns/
---
## InsertColumns(int, int) {#insertcolumns}

Insère plusieurs colonnes dans la feuille de calcul.

```csharp
public void InsertColumns(int columnIndex, int totalColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index de colonne. |
| totalColumns | Int32 | Le nombre de colonnes. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Insérer 3 colonnes à partir de l'index de colonne 1 (deuxième colonne)
            worksheet.Cells.InsertColumns(1, 3);
            
            // Ajouter des données d'exemple pour démontrer les colonnes insérées
            worksheet.Cells["A1"].PutValue("Original Column");
            worksheet.Cells["B1"].PutValue("Inserted Column 1");
            worksheet.Cells["C1"].PutValue("Inserted Column 2");
            worksheet.Cells["D1"].PutValue("Inserted Column 3");
            worksheet.Cells["E1"].PutValue("Original Column 2");
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, bool) {#insertcolumns_2}

Insère plusieurs colonnes dans la feuille de calcul.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, bool updateReference)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index de colonne. |
| totalColumns | Int32 | Le nombre de colonnes. |
| updateReference | Boolean | Indique si les références dans d'autres feuilles de calcul seront mises à jour. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Insérer 3 colonnes à l'index de colonne 2 (base 0), en décalant les colonnes existantes vers la droite
            worksheet.Cells.InsertColumns(2, 3, true);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, InsertOptions) {#insertcolumns_1}

Insère plusieurs colonnes dans la feuille de calcul.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, InsertOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index de colonne. |
| totalColumns | Int32 | Le nombre de colonnes. |
| options | InsertOptions | Les options pour l'opération d'insertion. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32InsertOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");

            // Créer des options d'insertion
            InsertOptions options = new InsertOptions();
            options.CopyFormatType = CopyFormatType.Clear;

            // Insérer une colonne à l'index 1 (deuxième colonne)
            worksheet.Cells.InsertColumns(1, 1, options);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


