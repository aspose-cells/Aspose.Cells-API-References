---
title: "WorkbookDesigner.Workbook"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "WorkbookDesigner propriété. Obtient et définit l'objet Workbook"
type: docs
url: /fr/net/aspose.cells/workbookdesigner/workbook/
---
## WorkbookDesigner.Workbook property

Obtient et définit l'objet `Workbook`.

```csharp
public Workbook Workbook { get; set; }
```

### Exemples

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Person1
    {
        public string Name { get; set; }
        public int Age { get; set; }

        public Person1(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }

    public class WorkbookDesignerPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Créer un nouveau concepteur de classeur
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Définir la propriété workbook avec un nouveau classeur
            designer.Workbook = new Workbook();
            
            // Ajouter une feuille de calcul et quelques marqueurs de modèle
            Worksheet worksheet = designer.Workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&Person.Name");
            worksheet.Cells["B1"].PutValue("&Person.Age");

            // Créer une source de données
            List<Person1> persons = new List<Person1>
            {
                new Person1("John", 25),
                new Person1("Mary", 30)
            };

            // Définir la source de données et traiter
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Afficher les résultats
            Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue); // Should output "John"
            Console.WriteLine("B2: " + worksheet.Cells["B2"].IntValue);   // Should output 25
            Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue); // Should output "Mary"
            Console.WriteLine("B3: " + worksheet.Cells["B3"].IntValue);   // Should output 30

            // Enregistrez le classeur
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


