---
title: "SmartTagProperty.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SmartTagProperty. Obtient et définit le nom de la propriété"
type: docs
url: /fr/net/aspose.cells.markup/smarttagproperty/name/
---
## SmartTagProperty.Name property

Obtient et définit le nom de la propriété.

```csharp
public string Name { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Markup;
    using System;
    using System.Reflection;

    public class SmartTagPropertyPropertyNameDemo
    {
        public static void Run()
        {
            try
            {
                // Crée une instance de SmartTagProperty en utilisant la réflexion puisque le constructeur n'est pas public
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Définir la propriété Name
                property.Name = "Department";

                // Afficher la valeur actuelle de la propriété Name
                Console.WriteLine("SmartTagProperty Name: " + property.Name);

                // Démontrez la modification de la propriété Name
                property.Name = "Project";
                Console.WriteLine("Updated SmartTagProperty Name: " + property.Name);

                // Montrez que la propriété peut être lue et modifiée
                Console.WriteLine("Name property demonstration completed successfully");
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


