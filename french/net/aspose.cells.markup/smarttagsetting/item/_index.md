---
title: "SmartTagSetting.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SmartTagSetting. Obtient un objet SmartTagCollection par l'index"
type: docs
url: /fr/net/aspose.cells.markup/smarttagsetting/item/
---
## SmartTagSetting indexer (1 of 3)

Obtient un objet [`SmartTagCollection`](../../smarttagcollection/) par l'index.

```csharp
public SmartTagCollection this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| index | L'index de l'objet [`SmartTagCollection`](../../smarttagcollection/) dans la liste. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Aspose");
            sheet.Cells["A2"].PutValue("Cells");

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            
            // Démontrer l'utilisation de la propriété Item
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
            smartTags.Add("http://docs.aspose.com", "docs");
            
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Version", "1.0");

            workbook.Save("SmartTagPropertyDemo.xlsx");
            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
    }
}
```

### Voir aussi

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (2 of 3)

Obtient l'objet [`SmartTagCollection`](../../smarttagcollection/) de la cellule.

```csharp
public SmartTagCollection this[int row, int column] { get; }
```

| Paramètre | Description |
| --- | --- |
| ligne | L'index de ligne de la cellule. |
| column | L'index de colonne de la cellule |

### Valeur de retour

Renvoie l'objet [`SmartTagCollection`](../../smarttagcollection/) de la cellule. Renvoie null s'il n'y a aucun smart tag sur la cellule.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            smartTagSetting.Add(0, 0); // Add smart tag to cell A1

            // Démontrer l'utilisation de la propriété Item
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart tags in cell A1: " + smartTagCollection.Count);
            Console.WriteLine("Namespace URI: " + smartTagCollection[0].Uri);
            Console.WriteLine("Tag name: " + smartTagCollection[0].Name);

            workbook.Save("SmartTagDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (3 of 3)

Obtient l'objet [`SmartTagCollection`](../../smarttagcollection/) de la cellule.

```csharp
public SmartTagCollection this[string cellName] { get; }
```

| Paramètre | Description |
| --- | --- |
| cellName | Le nom de la cellule. |

### Valeur de retour

Renvoie l'objet [`SmartTagCollection`](../../smarttagcollection/) de la cellule. Renvoie null s'il n'y a aucun smart tag sur la cellule.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingPropertyItemDemo2
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Obtenir la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Accédez au SmartTagSetting de la feuille de calcul
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;

                // Ajoutez un smart tag à la cellule A1 (ligne 0, colonne 0)
                int smartTagIndex = smartTagSetting.Add(0, 0);

                // Démontrez l'utilisation de la propriété Item (indexeur)
                SmartTagCollection smartTagCollection = smartTagSetting[smartTagIndex];

                // Ajouter une smart tag à la collection
                smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

                // Affichez les informations sur le smart tag
                Console.WriteLine("Number of smart tags in collection: " + smartTagCollection.Count);
                if (smartTagCollection.Count > 0)
                {
                    Console.WriteLine("First smart tag URI: " + smartTagCollection[0].Uri);
                    Console.WriteLine("First smart tag name: " + smartTagCollection[0].Name);
                }

                // Enregistrez le classeur
                workbook.Save("SmartTagItemDemo.xlsx");
                Console.WriteLine("SmartTagItemDemo.xlsx created successfully.");
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

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


