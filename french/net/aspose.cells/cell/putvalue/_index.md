---
title: "Cell.PutValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Insère une valeur booléenne dans la cellule"
type: docs
url: /fr/net/aspose.cells/cell/putvalue/
---
## PutValue(bool) {#putvalue}

Place une valeur booléenne dans la cellule.

```csharp
public void PutValue(bool boolValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| boolValue | Boolean |  |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Insérer une valeur booléenne dans la cellule B3 (ligne 2, colonne 2)
            cells[2, 2].PutValue(true);

            // Vérifier que la valeur a été définie correctement
            Console.WriteLine("Cell B3 value: " + cells[2, 2].Value);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(int) {#putvalue_2}

Place une valeur entière dans la cellule.

```csharp
public void PutValue(int intValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| intValue | Int32 | Valeur d'entrée |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Utilisation de PutValue avec des paramètres Int32
            cells[0, 0].PutValue(10);
            cells[1, 0].PutValue(20);
            cells[2, 0].PutValue(30);
            
            // Calculer la somme des valeurs
            cells[3, 0].Formula = "=SUM(A1:A3)";
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of values: " + cells[3, 0].IntValue);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(double) {#putvalue_1}

Place une valeur double dans la cellule.

```csharp
public void PutValue(double doubleValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| doubleValue | Double | Valeur d'entrée |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Insérer des valeurs double en utilisant la méthode PutValue
            cells[0, 0].PutValue("Item");
            cells[0, 1].PutValue("Price");
            cells[1, 0].PutValue("Apple");
            cells[1, 1].PutValue(0.69);
            cells[2, 0].PutValue("Banana");
            cells[2, 1].PutValue(0.49);
            cells[3, 0].PutValue("Orange");
            cells[3, 1].PutValue(0.29);

            // Enregistrez le classeur
            workbook.Save("PutValueWithDoubleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool, bool) {#putvalue_7}

Place une valeur dans la cellule ; si approprié, la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stringValue | String | Valeur d'entrée |
| isConverted | Boolean | Vrai: converti en un autre type de données si approprié. |
| setStyle | Boolean | Vrai: définir le format numérique sur le style de la cellule lors de la conversion en un autre type de données |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenir la cellule B3
            Cell cell = worksheet.Cells["B3"];
            
            // Définir la validation des données pour l'âge (doit être un nombre positif)
            Validation validation = cell.GetValidation();
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "0";
            
            // Insérer la valeur avec conversion et vérification de validation
            cell.PutValue("-60", true, false);
            
            // Calculer les formules (bien que non nécessaire dans ce cas simple)
            workbook.CalculateFormula();
            
            // Vérifier si la valeur est valide
            bool isValid = cell.GetValidationValue();
            Console.WriteLine("Is value valid? " + isValid);
            
            // Enregistrer le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool) {#putvalue_6}

Place une valeur chaîne dans la cellule et convertit la valeur en un autre type de données si approprié.

```csharp
public void PutValue(string stringValue, bool isConverted)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stringValue | String | Valeur d'entrée |
| isConverted | Boolean | Vrai: converti en un autre type de données si approprié. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Démontrer PutValue avec des paramètres string et booléen
            cells["B2"].PutValue("123", true);  // String value with conversion flag
            cells["C2"].PutValue("456", false); // String value without conversion
            
            // Vérifier les valeurs
            Console.WriteLine("B2 value (converted): " + cells["B2"].Value); // Should show 123 as number
            Console.WriteLine("C2 value (raw): " + cells["C2"].Value);       // Should show "456" as string

            workbook.Save("PutValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string) {#putvalue_5}

Place une valeur chaîne dans la cellule.

```csharp
public void PutValue(string stringValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stringValue | String | Valeur d'entrée |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Utilisation de PutValue avec des paramètres string
            cells[0, 0].PutValue("Product");
            cells[0, 1].PutValue("Category");
            cells[0, 2].PutValue("Price");
            
            cells[1, 0].PutValue("Laptop");
            cells[1, 1].PutValue("Electronics");
            cells[1, 2].PutValue(999.99);
            
            cells[2, 0].PutValue("Desk Chair");
            cells[2, 1].PutValue("Furniture");
            cells[2, 2].PutValue(199.50);
            
            // Enregistrez le classeur
            workbook.Save("PutValueStringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(DateTime) {#putvalue_3}

Place une valeur DateTime dans la cellule.

```csharp
public void PutValue(DateTime dateTime)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dateTime | DateTime | Valeur d'entrée |

### Remarques

Définir une valeur DateTime pour une cellule ne signifie pas que la cellule sera automatiquement formatée en date/heure. La valeur DateTime était conservée comme valeur numérique dans le modèle de données à la fois de MS Excel et d'Aspose.Cells. Le fait que la valeur numérique soit interprétée comme une valeur numérique ou comme une date/heure dépend du format numérique appliqué à cette cellule. Si cette cellule n'est pas formatée en date/heure, elle sera affichée comme une valeur numérique même si ce que vous avez saisi est une DateTime.

### Exemples

Cet exemple montre comment définir une valeur DateTime dans une cellule et la faire afficher en date/heure.

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Insérer une date/heure dans une cellule
Cell cell = cells[0, 0];
cell.PutValue(new DateTime(2023, 5, 15));
Style style = cell.GetStyle(false);
style.Number = 14;
cell.SetStyle(style);
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(object) {#putvalue_4}

Place une valeur d'objet dans la cellule.

```csharp
public void PutValue(object objectValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| objectValue | Object | valeur d'entrée |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // PutValue avec un objet DateTime
            DateTime dt = new DateTime(2008, 2, 2);
            cells[0, 0].PutValue((object)dt);
            
            // PutValue avec un objet string
            cells[1, 0].PutValue((object)"Hello World");
            
            // PutValue avec un objet numeric
            cells[2, 0].PutValue((object)123.45);
            
            // Enregistrez le classeur
            workbook.Save("PutValueWithObjectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


