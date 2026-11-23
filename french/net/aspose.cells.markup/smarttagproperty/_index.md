---
title: "Classe SmartTagProperty"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Markup.SmartTagProperty classe. Représente la propriété du smart tag de cellule"
type: docs
url: /fr/net/aspose.cells.markup/smarttagproperty/
---
## SmartTagProperty class

Représente la propriété de la balise intelligente de la cellule.

```csharp
public class SmartTagProperty
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Name](../../aspose.cells.markup/smarttagproperty/name/) { get; set; } | Obtient et définit le nom de la propriété. |
| [Value](../../aspose.cells.markup/smarttagproperty/value/) { get; set; } | Obtient et définit la valeur de la propriété. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagPropertyDemo
    {
        public static void Run()
        {
            try
            {
                // Crée une instance de SmartTagProperty en utilisant la réflexion puisque le constructeur n'est pas public
                var smartTagProperty = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Définissez les propriétés Name et Value
                smartTagProperty.Name = "DocumentType";
                smartTagProperty.Value = "FinancialReport";

                // Affiche les valeurs des propriétés
                Console.WriteLine($"SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"SmartTagProperty Value: {smartTagProperty.Value}");

                // Démontre la modification des propriétés
                smartTagProperty.Name = "Status";
                smartTagProperty.Value = "Approved";

                Console.WriteLine($"Updated SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"Updated SmartTagProperty Value: {smartTagProperty.Value}");

                Console.WriteLine("SmartTagProperty demonstration completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SmartTagProperty: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


