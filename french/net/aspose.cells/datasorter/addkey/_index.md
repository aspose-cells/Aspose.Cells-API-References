---
title: "DataSorter.AddKey"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode DataSorter. Ajoute l'index de la colonne triée et l'ordre de tri"
type: docs
url: /fr/net/aspose.cells/datasorter/addkey/
---
## AddKey(int, SortOrder) {#addkey_1}

Ajoute l'index de colonne triée et l'ordre de tri.

```csharp
public void AddKey(int key, SortOrder order)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| clé | Int32 | L'index de la colonne triée (position absolue, la colonne A est 0, B est 1, ...) |
| ordre | SortOrder | L'ordre de tri |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Ajouter une clé de tri pour la colonne B (index 1) avec un ordre croissant
            workbook.DataSorter.AddKey(1, SortOrder.Ascending);
            
            // Trier la plage de données (A1:B4)
            workbook.DataSorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // Afficher les valeurs triées
            Console.WriteLine("Sorted by Age (Ascending):");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[$"A{i+1}"].StringValue}: {worksheet.Cells[$"B{i+1}"].IntValue}");
            }
        }
    }
}
```

### Voir aussi

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string) {#addkey_2}

Ajoute l'index de colonne triée et l'ordre de tri avec une liste de tri personnalisée.

```csharp
public void AddKey(int key, SortOrder order, string customList)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| clé | Int32 | L'index de la colonne triée (position absolue, la colonne A est 0, B est 1, ...) |
| ordre | SortOrder | L'ordre de tri. |
| customList | String | La liste de tri personnalisée. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Données d'exemple à trier
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("ddd");
            worksheet.Cells["A3"].PutValue("aaa");
            worksheet.Cells["A4"].PutValue("ccc");
            worksheet.Cells["A5"].PutValue("bbb");

            // Créer un trieur de données et ajouter une clé de tri personnalisée
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending, "aaa,ddd,ccc,bbb");
            sorter.HasHeaders = true;

            // Trier les données
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // Enregistrer le résultat
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOnType, SortOrder, object) {#addkey}

Ajoute l'index de colonne triée et l'ordre de tri avec une liste de tri personnalisée.

```csharp
public void AddKey(int key, SortOnType type, SortOrder order, object customList)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| clé | Int32 | L'index de la colonne triée (position absolue, la colonne A est 0, B est 1, ...) |
| type | SortOnType | Le type de valeur triée. |
| ordre | SortOrder | L'ordre de tri. |
| customList | Object | La liste de tri personnalisée. |

### Remarques

Si le type est SortOnType.CellColor ou SortOnType.FontColor, la customList est Color.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Créer un trieur de données
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;

            try
            {
                // Appeler AddKey avec les paramètres : (Int32, SortOnType, SortOrder, Object)
                sorter.AddKey(
                    1,                          // Column index (B column)
                    SortOnType.Value,           // Sort on values (fixed from Values to Value)
                    SortOrder.Ascending,        // Sort order
                    null                        // Custom list (null for default)
                );

                // Définir la plage à trier
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 3;
                area.EndColumn = 1;

                // Trier les données
                sorter.Sort(worksheet.Cells, area);

                Console.WriteLine("Data sorted successfully using AddKey with parameters (Int32, SortOnType, SortOrder, Object)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddKey method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string[]) {#addkey_3}

Ajoute l'index de colonne triée et l'ordre de tri avec une liste de tri personnalisée.

```csharp
public void AddKey(int key, SortOrder order, string[] customList)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| clé | Int32 | L'index de la colonne triée (position absolue, la colonne A est 0, B est 1, ...) |
| ordre | SortOrder | L'ordre de tri. |
| customList | String[] | La liste de tri personnalisée. |

### Voir aussi

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


