---
title: "HtmlTableLoadOptionCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode HtmlTableLoadOptionCollection. Ajoute un HtmlTableLoadOption à cette collection"
type: docs
url: /fr/net/aspose.cells/htmltableloadoptioncollection/add/
---
## Add(HtmlTableLoadOption) {#add}

Ajoute un HtmlTableLoadOption à cette collection.

```csharp
[Obsolete("Use HtmlTableLoadOptionCollection.AddTableLoadOption(HtmlTableLoadOption) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(HtmlTableLoadOption item)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| élément | HtmlTableLoadOption | un HtmlTableLoadOption |

### Valeur de retour

l'index de l'élément ajouté

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode AddTableLoadOption(). Cette méthode sera supprimée 6 mois plus tard, à compter de décembre 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithHtmlTableLoadOptionDemo
    {
        public static void Run()
        {
            // Créer des options de chargement HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Ajouter des options de chargement du tableau
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption1);

            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // Charger le classeur avec des options
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Enregistrer la sortie
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add_1}

Ajoutez un HtmlTableLoadOption à la liste.

```csharp
public int Add(int tableIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tableIndex | Int32 | Index du tableau |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            // Créez HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Accédez à l'instance HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Ajouter une nouvelle HtmlTableLoadOption par indice de tableau
            int index = tableLoadOptions.Add(0);

            // Accéder au HtmlTableLoadOption ajouté
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;

            // Créer un classeur et charger le HTML avec des options
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_4}

Ajoutez un HtmlTableLoadOption à la liste.

```csharp
public int Add(string tableId)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tableId | String | ID du tableau |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Créez HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Accédez à l'instance HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Ajouter une nouvelle HtmlTableLoadOption par identifiant de tableau
            int index = tableLoadOptions.Add("mainTable");

            // Accéder au HtmlTableLoadOption ajouté
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;
            option.TargetSheetIndex = 0;

            // Créer le classeur et charger le HTML avec des options
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_2}

Ajoutez un HtmlTableLoadOption à la liste.

```csharp
public int Add(int tableIndex, int targetSheetIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tableIndex | Int32 | Index du tableau |
| targetSheetIndex | Int32 | L’index cible de la feuille de calcul dans Excel |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer des options de chargement HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Ajouter des tableaux par index avec l’index de feuille cible
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 to sheet index 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 to sheet index 0
            loadOptions.TableLoadOptions.Add(2, 1); // Table index 2 to sheet index 1

            // Charger le fichier HTML avec les options spécifiées
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_5}

Ajoutez un HtmlTableLoadOption à la liste.

```csharp
public int Add(string tableId, int targetSheetIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tableId | String | ID du tableau |
| targetSheetIndex | Int32 | L’index cible de la feuille de calcul dans Excel |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Demo
    {
        public static void Run()
        {
            // Créez HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Accédez à l'instance HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Ajouter une nouvelle HtmlTableLoadOption par identifiant de tableau et indice de feuille cible
            int index = tableLoadOptions.Add("tableId", 1);

            // Créer un classeur et charger le HTML avec des options
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int) {#add_3}

Ajoutez un HtmlTableLoadOption à la liste.

```csharp
public int Add(int tableIndex, int targetSheetIndex, int originalSheetIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tableIndex | Int32 | Index du tableau |
| targetSheetIndex | Int32 | L’index cible de la feuille de calcul dans Excel |
| originalSheetIndex | Int32 | L’index d’origine de la feuille de calcul dans le HTML |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Créez HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Accéder à la HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Ajouter un tableau avec l’index 1, l’index de feuille cible 1 et l’index de feuille d’origine 0
            int addedIndex = tableLoadOptions.Add(1, 1, 0);

            // Créer un classeur et charger le HTML avec des options
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Enregistrer le résultat
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add_6}

Ajoutez un HtmlTableLoadOption à la liste.

```csharp
public int Add(string tableId, int targetSheetIndex, int originalSheetIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tableId | String | ID du tableau |
| targetSheetIndex | Int32 | L’index cible de la feuille de calcul dans Excel |
| originalSheetIndex | Int32 | L’index d’origine de la feuille de calcul dans le HTML |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Démontrer la méthode Add avec les paramètres (String, Int32, Int32)
            int addedIndex = tableLoadOptions.Add("sampleTable", 1, 0);
            
            HtmlTableLoadOption option = tableLoadOptions[addedIndex];
            option.TableToListObject = true;

            // Charger le fichier HTML (remplacez par le chemin réel du fichier)
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


