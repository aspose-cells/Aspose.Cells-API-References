---
title: "RowCollection.GetEnumerator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode RowCollection. Obtient un énumérateur qui parcourt les lignes de cette collection"
type: docs
url: /fr/net/aspose.cells/rowcollection/getenumerator/
---
## GetEnumerator() {#getenumerator}

Obtient un énumérateur qui parcourt les lignes de cette collection

```csharp
public IEnumerator GetEnumerator()
```

### Valeur de retour

L'énumérateur de lignes qui parcourra toutes les lignes existantes dans cette collection.

### Exemples

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir les hauteurs de lignes pour la démonstration
            worksheet.Cells.SetRowHeight(0, 15);
            worksheet.Cells.SetRowHeight(1, 20);
            worksheet.Cells.SetRowHeight(2, 25);

            IEnumerator enumerator = worksheet.Cells.Rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine($"Row index: {row.Index}, Height: {row.Height}");
            }
        }
    }
}
```

### Voir aussi

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

Obtient un énumérateur qui parcourt les lignes de cette collection

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| inversé | Boolean | si les lignes doivent être énumérées dans l'ordre inversé |
| synchronisation | Boolean | si l'énumérateur retourné doit vérifier la modification de la collection de lignes et rester synchronisé avec elle. |

### Valeur de retour

L'énumérateur de lignes qui parcourra toutes les lignes existantes dans cette collection.

### Remarques

Si la collection de lignes est modifiée (par des opérations pouvant entraîner l'instanciation d'une nouvelle Row ou la suppression d'une Row existante) pendant le parcours avec l'énumérateur, un énumérateur synchronisé doit être utilisé à la place d'un énumérateur normal afin que le parcours puisse continuer à partir de la position immédiatement après celle qui a été parcourue par le dernier MoveNext(). Cependant, en plus de l'avantage qu'aucun élément ne soit sauté ou parcouru plusieurs fois, l'inconvénient de l'énumérateur synchronisé est que les performances seront légèrement dégradées comparées à celles d'un énumérateur normal.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple aux lignes
            for (int i = 0; i < 5; i++)
            {
                Row row = worksheet.Cells.Rows[i];
                row[0].PutValue($"Row {i + 1}");
            }
            
            try
            {
                // Obtenir la RowCollection
                RowCollection rows = worksheet.Cells.Rows;
                
                // Appeler GetEnumerator avec les paramètres (reversed: true, sync: false)
                IEnumerator enumerator = rows.GetEnumerator(true, false);
                
                Console.WriteLine("Iterating rows in reverse order:");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
                
                // Appeler GetEnumerator avec les paramètres (reversed: false, sync: true)
                enumerator = rows.GetEnumerator(false, true);
                
                Console.WriteLine("\nIterating rows in normal order (synchronized):");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("RowCollectionGetEnumeratorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


