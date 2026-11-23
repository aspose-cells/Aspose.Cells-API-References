---
title: "WorkbookDesigner.ClearDataSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "WorkbookDesigner méthode. Efface toutes les sources de données"
type: docs
url: /fr/net/aspose.cells/workbookdesigner/cleardatasource/
---
## WorkbookDesigner.ClearDataSource method

Efface toutes les sources de données.

```csharp
public void ClearDataSource()
```

### Exemples

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }

        public Person(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }

    public class WorkbookDesignerMethodClearDataSourceDemo
    {
        public static void Run()
        {
            WorkbookDesigner designer = new WorkbookDesigner();
            Worksheet worksheet = designer.Workbook.Worksheets[0];

            // Créer des données d'exemple
            List<Person> persons = new List<Person>
            {
                new Person("John", 30),
                new Person("Mary", 25),
                new Person("Peter", 35)
            };

            // Configurer les marqueurs intelligents
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("&=Person.Name");
            worksheet.Cells["B2"].PutValue("&=Person.Age");

            // Première liaison de données
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Effacer la source de données et relier à nouveau
            designer.ClearDataSource();
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Enregistrer le résultat
            designer.Workbook.Save("ClearedDataSourceOutput.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


