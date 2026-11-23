---
title: "Cells.InsertRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Insère plusieurs lignes dans la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/cells/insertrows/
---
## InsertRows(int, int, bool) {#insertrows_2}

Insère plusieurs lignes dans la feuille de calcul.

```csharp
public void InsertRows(int rowIndex, int totalRows, bool updateReference)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index de ligne. |
| totalRows | Int32 | Nombre de lignes à insérer. |
| updateReference | Boolean | Indique si les références dans d'autres feuilles de calcul seront mises à jour. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            worksheet.Cells["A4"].PutValue("Data 3");
            
            // Insérer une ligne à l'index 2 (deviendra la nouvelle ligne 3)
            worksheet.Cells.InsertRows(2, 1, true);
            
            // Ajouter des données à la ligne insérée
            worksheet.Cells["A3"].PutValue("Inserted Data");
            
            // Enregistrez le classeur
            workbook.Save("InsertRowsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int, InsertOptions) {#insertrows_1}

Insère plusieurs lignes dans la feuille de calcul.

```csharp
public void InsertRows(int rowIndex, int totalRows, InsertOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index de ligne. |
| totalRows | Int32 | Nombre de lignes à insérer. |
| options | InsertOptions | Options pour l'opération d'insertion. |

### Exemples

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32InsertOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // Insérer 3 lignes à l'index de ligne 5 avec les options spécifiées
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            workbook.Save("InsertRowsWithOptions.xlsx");
        }
    }
}
```

### Voir aussi

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int) {#insertrows}

Insère plusieurs lignes dans la feuille de calcul.

```csharp
public void InsertRows(int rowIndex, int totalRows)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index de ligne. |
| totalRows | Int32 | Nombre de lignes à insérer. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajoutez des données d'exemple
            cells["A1"].PutValue("Header1");
            cells["B1"].PutValue("Header2");
            cells["A2"].PutValue("Data1");
            cells["B2"].PutValue("Data2");
            cells["A3"].PutValue("Data3");
            cells["B3"].PutValue("Data4");

            // Insérer 2 lignes à l'index de ligne 2
            cells.InsertRows(2, 2);

            // Vérifier que les lignes insérées sont vides
            Console.WriteLine("Cell A2 value: " + cells[1, 0].Value); // Should be "Data1"
            Console.WriteLine("Cell A3 value: " + cells[2, 0].Value); // Should be null (empty)
            Console.WriteLine("Cell A4 value: " + cells[3, 0].Value); // Should be null (empty)
            Console.WriteLine("Cell A5 value: " + cells[4, 0].Value); // Should be "Data3"

            // Enregistrez le classeur
            workbook.Save("InsertRowsDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


