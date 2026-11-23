---
title: "Row.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Row. Vérifie si cet objet fait référence à la même ligne qu'un autre"
type: docs
url: /fr/net/aspose.cells/row/equals/
---
## Equals(object) {#equals_1}

Vérifie si cet objet fait référence à la même ligne qu'un autre.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Object | un autre objet |

### Valeur de retour

true si deux objets font référence à la même ligne.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créez deux lignes à comparer
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];
            
            // Définissez certaines propriétés pour différencier les lignes
            row1.Height = 20;
            row2.Height = 25;
            
            try
            {
                // Appelez la méthode Equals avec le paramètre Object
                bool result1 = row1.Equals((object)row2);
                Console.WriteLine($"Comparing row1 with row2: {result1}");
                
                // Comparez row1 avec elle-même
                bool result2 = row1.Equals((object)row1);
                Console.WriteLine($"Comparing row1 with itself: {result2}");
                
                // Comparer avec null
                bool result3 = row1.Equals((object)null);
                Console.WriteLine($"Comparing row1 with null: {result3}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
            
            workbook.Save("RowMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Row) {#equals}

Vérifie si cet objet fait référence à la même ligne qu'un autre objet ligne.

```csharp
public bool Equals(Row row)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Row | un autre objet de ligne |

### Valeur de retour

vrai si deux objets de ligne font référence à la même ligne.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez deux lignes à comparer
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];

            // Définissez certaines propriétés pour différencier les lignes
            row1.Height = 20;
            row2.Height = 25;
            row1.IsHidden = false;
            row2.IsHidden = true;

            try
            {
                // Appelez la méthode Equals pour comparer les lignes
                bool areEqual = row1.Equals(row2);

                // Afficher le résultat
                Console.WriteLine($"Are rows equal? {areEqual}");

                // Créez un autre objet de ligne avec les mêmes propriétés que row1
                Row row3 = worksheet.Cells.Rows[2];
                row3.Height = row1.Height;
                row3.IsHidden = row1.IsHidden;

                // Comparez row1 avec row3 (devrait être égal)
                bool areEqual2 = row1.Equals(row3);
                Console.WriteLine($"Are rows equal after matching properties? {areEqual2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("RowEqualsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


