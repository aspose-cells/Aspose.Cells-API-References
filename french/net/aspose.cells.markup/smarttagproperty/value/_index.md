---
title: "SmartTagProperty.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SmartTagProperty. Obtient et définit la valeur de la propriété"
type: docs
url: /fr/net/aspose.cells.markup/smarttagproperty/value/
---
## SmartTagProperty.Value property

Obtient et définit la valeur de la propriété.

```csharp
public string Value { get; set; }
```

### Exemples

```csharp
using Aspose.Cells.Markup;
using System;

namespace AsposeCellsExamples
{
    public class SmartTagPropertyPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Créez une instance de SmartTagProperty en utilisant le constructeur non‑public
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Définissez le nom et la valeur de la propriété
                property.Name = "Category";
                property.Value = "Finance";

                // Affiche les valeurs des propriétés
                Console.WriteLine($"SmartTagProperty Name : {property.Name}");
                Console.WriteLine($"SmartTagProperty Value: {property.Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SmartTagProperty](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


