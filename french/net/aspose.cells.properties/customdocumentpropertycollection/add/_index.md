---
title: "CustomDocumentPropertyCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "CustomDocumentPropertyCollection method. Crée une nouvelle propriété de document personnalisée du type de données PropertyType.String"
type: docs
url: /fr/net/aspose.cells.properties/customdocumentpropertycollection/add/
---
## Add(string, string) {#add_4}

Crée une nouvelle propriété de document personnalisée du type de données **PropertyType.String**.

```csharp
public DocumentProperty Add(string name, string value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la propriété. |
| valeur | String | La valeur de la propriété. |

### Valeur de retour

Le nouvel objet de propriété créé.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.CustomDocumentProperties.Add("startdate", "ToneyTest");
            
            Console.WriteLine("Custom Property Value: " + 
                workbook.CustomDocumentProperties["startdate"].Value);
                
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_2}

Crée une nouvelle propriété de document personnalisée du type de données **PropertyType.Number**.

```csharp
public DocumentProperty Add(string name, int value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la propriété. |
| valeur | Int32 | La valeur de la propriété. |

### Valeur de retour

Le nouvel objet de propriété créé.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet1");
            
            // Ajouter des propriétés de document personnalisées
            workbook.CustomDocumentProperties.Add("textProperty", "Sample Text");
            workbook.CustomDocumentProperties.Add("numericProperty", 42);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Vérifier les propriétés
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Text Property Value: " + loadedWorkbook.CustomDocumentProperties["textProperty"].Value);
            Console.WriteLine("Numeric Property Value: " + loadedWorkbook.CustomDocumentProperties["numericProperty"].Value);
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, DateTime) {#add_3}

Crée une nouvelle propriété de document personnalisée du type de données **PropertyType.DateTime**.

```csharp
public DocumentProperty Add(string name, DateTime value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la propriété. |
| valeur | DateTime | La valeur de la propriété. |

### Valeur de retour

Le nouvel objet de propriété créé.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Properties;

    public class CustomDocumentPropertyCollectionMethodAddWithStringDateTimeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Obtenir la collection des propriétés de document personnalisées
            CustomDocumentPropertyCollection customProps = workbook.Worksheets.CustomDocumentProperties;

            try
            {
                // Ajouter une propriété DateTime
                DateTime currentTime = DateTime.Now;
                DocumentProperty addedProp = customProps.Add("ReportGenerated", currentTime);

                // Afficher les informations sur la propriété ajoutée
                Console.WriteLine($"Property Name : {addedProp.Name}");
                Console.WriteLine($"Property Type : {addedProp.Type}");
                Console.WriteLine($"Property Value: {addedProp.ToDateTime():O}");

                // Enregistrer le classeur (facultatif, montre que la propriété persiste)
                workbook.Save("AddDateTimePropertyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding DateTime property: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool) {#add}

Crée une nouvelle propriété de document personnalisée du type de données **PropertyType.Boolean**.

```csharp
public DocumentProperty Add(string name, bool value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la propriété. |
| valeur | Boolean | La valeur de la propriété. |

### Valeur de retour

Le nouvel objet de propriété créé.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;

            // Ajouter une propriété personnalisée booléenne
            customProperties.Add("IsApproved", true);

            // Afficher la propriété ajoutée
            DocumentProperty property = customProperties["IsApproved"];
            Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");

            // Enregistrez le classeur
            workbook.Save("CustomPropertiesExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, double) {#add_1}

Crée une nouvelle propriété de document personnalisée du type de données **PropertyType.Float**.

```csharp
public DocumentProperty Add(string name, double value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la propriété. |
| valeur | Double | La valeur de la propriété. |

### Valeur de retour

Le nouvel objet de propriété créé.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddWithStringDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Démontrer la méthode Add avec des paramètres String et Double
            customProperties.Add("Rating", 4.5);
            customProperties.Add("Score", 8.75);

            // Accéder et afficher les propriétés ajoutées
            DocumentProperty ratingProperty = customProperties["Rating"];
            DocumentProperty scoreProperty = customProperties["Score"];

            Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
            Console.WriteLine($"Score: {scoreProperty.ToDouble()}");

            workbook.Save("CustomDocumentPropertiesWithDoubleValues.xlsx");
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


