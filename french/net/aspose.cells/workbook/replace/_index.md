---
title: "Workbook.Replace"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Remplace la valeur d’une cellule par une nouvelle chaîne"
type: docs
url: /fr/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

Remplace la valeur d'une cellule par une nouvelle chaîne.

```csharp
public int Replace(string placeHolder, string newValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| newValue | String | Valeur String à remplacer |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Apple Orange");
            
            // Remplacer toutes les occurrences de "Apple" par "Mango"
            workbook.Replace("Apple", "Mango");
            
            // Enregistrez le classeur
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

Remplace la valeur d'une cellule par un nouvel entier.

```csharp
public int Replace(string placeHolder, int newValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| newValue | Int32 | Valeur Integer à remplacer |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul et ajouter des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("OriginalValue");
            worksheet.Cells["A2"].PutValue("OriginalValue");
            worksheet.Cells["A3"].PutValue("OriginalValue");
            
            // Remplacez toutes les occurrences de "OriginalValue" par l'entier 100
            workbook.Replace("OriginalValue", 100);
            
            // Enregistrez le classeur
            workbook.Save("ReplacedWorkbook.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

Remplace la valeur d'une cellule par un nouveau double.

```csharp
public int Replace(string placeHolder, double newValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| newValue | Double | Valeur double à remplacer |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Mettez des données d'exemple dans les cellules
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnotherOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Remplacez le texte par une valeur double
            double newValue = 100.0;
            workbook.Replace("AnOldValue", newValue);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

Remplace la valeur d'une cellule par un nouveau tableau de chaînes.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| newValues | String[] | Tableau de chaînes à remplacer |
| isVertical | Boolean | Vrai - Vertical, Faux - Horizontal |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Définissez les nouvelles valeurs à utiliser pour le remplacement
            string[] newValues = new string[] { "Tom", "Alice", "Jerry" };
            
            // Remplacez toutes les occurrences de "AnOldValue" par les nouvelles valeurs
            workbook.Replace("AnOldValue", newValues, true);
            
            // Enregistrez le classeur
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

Remplace les valeurs des cellules par un tableau d'entiers.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| newValues | Int32[] | Tableau d'entiers à remplacer |
| isVertical | Boolean | Vrai - Vertical, Faux - Horizontal |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("OldValue");
            worksheet.Cells["A2"].PutValue("OldValue");
            worksheet.Cells["A3"].PutValue("OtherValue");
            
            // Définissez les valeurs de remplacement
            int[] newValues = new int[] { 1, 2, 3 };
            
            // Remplacez "OldValue" par le tableau d'entiers
            workbook.Replace("OldValue", newValues, true);
            
            // Enregistrez le classeur
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

Remplace les valeurs des cellules par un tableau de doubles.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| newValues | Double[] | Tableau de doubles à remplacer |
| isVertical | Boolean | Vrai - Vertical, Faux - Horizontal |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Définissez les valeurs de remplacement
            double[] newValues = new double[] { 1.23, 2.56, 3.14159 };
            
            // Remplacez toutes les occurrences de "AnOldValue" par les nouvelles valeurs
            workbook.Replace("AnOldValue", newValues, true);
            
            // Enregistrez le classeur
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

Remplace les valeurs des cellules par des données provenant d'un DataTable.

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| insertTable | DataTable | DataTable à remplacer |

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDataTableDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créez un DataTable d'exemple
            DataTable dataTable = new DataTable("Customers");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("City", typeof(string));
            
            // Ajoutez des données d'exemple au DataTable
            dataTable.Rows.Add(1, "John Doe", "New York");
            dataTable.Rows.Add(2, "Jane Smith", "London");
            dataTable.Rows.Add(3, "Mike Johnson", "Paris");
            
            // Ajoutez du texte à la feuille de calcul qui sera remplacé
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("CustomerData");
            
            // Remplacez le texte par le DataTable
            workbook.Replace("CustomerData", dataTable);
            
            // Enregistrez le classeur
            workbook.Save("Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

Remplace les valeurs des cellules par de nouvelles données.

```csharp
public int Replace(bool boolValue, object newValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| boolValue | Boolean | La valeur booléenne à remplacer. |
| newValue | Object | Nouvelle valeur. Peut être une chaîne, un entier, un double ou une valeur DateTime. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithBooleanObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir certaines cellules avec des valeurs booléennes
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            worksheet.Cells["A3"].PutValue(true);
            
            try
            {
                // Appeler la méthode Replace pour remplacer toutes les valeurs 'true' par "REPLACED"
                int replacements = workbook.Replace(true, "REPLACED");
                
                Console.WriteLine($"Replaced {replacements} occurrences of 'true' with 'REPLACED'");
                
                // Affichez les résultats
                Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("WorkbookMethodReplaceWithBooleanObjectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

Remplace les valeurs des cellules par de nouvelles données.

```csharp
public int Replace(int intValue, object newValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| intValue | Int32 | La valeur entière à remplacer. |
| newValue | Object | Nouvelle valeur. Peut être une chaîne, un entier, un double ou une valeur DateTime. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithInt32ObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir certaines cellules avec des valeurs entières à remplacer
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(100);
            
            try
            {
                // Appeler la méthode Replace avec les paramètres (Int32, Object)
                int replacements = workbook.Replace(100, "ReplacedValue");
                
                Console.WriteLine($"Replaced {replacements} occurrences of the value 100");
                
                // Afficher le contenu de la feuille de calcul après le remplacement
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("WorkbookMethodReplaceWithInt32ObjectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

Remplace la valeur d'une cellule par une nouvelle chaîne.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| newValue | String | Valeur String à remplacer |
| options | ReplaceOptions | Les options de remplacement |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false
            };

            int replacedCount = workbook.Replace("Hello", "Hi", options);

            Console.WriteLine($"Replacements made: {replacedCount}");
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ReplaceOptions](../../replaceoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


