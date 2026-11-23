---
title: "Row.GetEnumerator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Row. Obtient l'énumérateur des cellules"
type: docs
url: /fr/net/aspose.cells/row/getenumerator/
---
## GetEnumerator() {#getenumerator}

Obtient l'énumérateur des cellules

```csharp
public IEnumerator GetEnumerator()
```

### Valeur de retour

L'énumérateur des cellules qui parcourra toutes les cellules existantes dans cette ligne.

### Exemples

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Remplir des données d'exemple
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            // Obtenir l'énumérateur pour la première ligne (ligne d'en-tête)
            IEnumerator en = cells.Rows[0].GetEnumerator();
            while (en.MoveNext())
            {
                Cell cell = (Cell)en.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }
        }
    }
}
```

### Voir aussi

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

Obtient un énumérateur qui parcourt les cellules de cette ligne.

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| inversé | Boolean | si l'énumération des cellules se fait dans l'ordre inverse |
| synchronisation | Boolean | si l'énumérateur retourné doit vérifier la modification des cellules dans cette ligne et rester synchronisé avec elle. |

### Valeur de retour

L'énumérateur des cellules qui parcourra toutes les cellules existantes dans cette ligne.

### Remarques

Si la ligne sera modifiée (par des opérations pouvant entraîner la création d'une nouvelle Cell ou la suppression d'une Cell existante) pendant le parcours avec l'énumérateur, le synchronized enumerator doit être utilisé à la place du normal enumerator afin que le parcours puisse continuer à la position juste après celle qui a été parcourue par le dernier MoveNext(). Cependant, en plus de l'avantage qu'aucun élément ne soit sauté ou parcouru à nouveau, le inconvénient du synchronized enumerator est que les performances seront légèrement dégradées comparées au normal enumerator.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données aux cellules de la première ligne
            Row row = worksheet.Cells.Rows[0];
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            try
            {
                // Appeler GetEnumerator avec reversed=false et sync=true
                IEnumerator enumerator = row.GetEnumerator(false, true);
                
                Console.WriteLine("Cells in row 1:");
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }

                // Appeler GetEnumerator avec reversed=true et sync=false pour démontrer l'itération inversée
                Console.WriteLine("\nCells in row 1 (reversed order):");
                enumerator = row.GetEnumerator(true, false);
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("RowMethodGetEnumeratorWithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


