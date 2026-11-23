---
title: "SmartTagSetting.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SmartTagSetting. Ajoute un objet SmartTagCollection à une cellule"
type: docs
url: /fr/net/aspose.cells.markup/smarttagsetting/add/
---
## Add(int, int) {#add}

Ajoute un objet [`SmartTagCollection`](../../smarttagcollection/) à une cellule.

```csharp
public int Add(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | La ligne de la cellule. |
| column | Int32 | La colonne de la cellule. |

### Valeur de retour

Renvoie l'index d'un objet [`SmartTagCollection`](../../smarttagcollection/) dans la feuille de calcul.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0); // Add to cell A1 (row 0, column 0)

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart Tags Count: " + smartTagSetting.Count.ToString());
            workbook.Save("SmartTagDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Ajoute des smart tags à la cellule.

```csharp
public int Add(string cellName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String | Le nom de la cellule. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenez l'instance SmartTagSetting
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            
            try
            {
                // Appelez la méthode Add avec le paramètre String
                int index = smartTagSetting.Add("A1");
                
                Console.WriteLine($"SmartTag added successfully at index: {index}");
                
                // Ajoutez du contenu pour démontrer l'effet
                worksheet.Cells["A1"].PutValue("This cell has a smart tag");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("SmartTagSettingMethodAddWithStringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


