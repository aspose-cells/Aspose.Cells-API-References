---
title: "OleObject.SetEmbeddedObject"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode OleObject. Définit les données de l'objet intégré"
type: docs
url: /fr/net/aspose.cells.drawing/oleobject/setembeddedobject/
---
## SetEmbeddedObject(bool, byte[], string, bool, string) {#setembeddedobject}

Définit les données de l'objet intégré.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| linkToFile | Boolean | Indique si l'objet est lié au fichier. Si vrai, le paramètre objectData est ignoré. |
| objectData | Byte[] | Les données de l'objet intégré. |
| sourceFileName | String | Le nom du fichier. |
| displayAsIcon | Boolean | Indique si l'objet est affiché sous forme d'icône. Si vrai, les données d'image originales seront recouvertes par l'icône. |
| label | String | Le libellé de l'icône. Fonctionne uniquement lorsque displayAsIcon est vrai. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un OleObject à la feuille de calcul
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Préparer les paramètres pour SetEmbeddedObject
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.xlsx");
                string sourceFileName = "sample.xlsx";
                bool displayAsIcon = false;
                string label = "Excel Document";

                // Appeler SetEmbeddedObject avec les paramètres spécifiés
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String)");
                
                // Afficher certaines propriétés pour montrer l'effet
                Console.WriteLine($"OleObject label: {oleObject.Label}");
                Console.WriteLine($"Display as icon: {oleObject.DisplayAsIcon}");
                Console.WriteLine($"Is linked to file: {oleObject.IsLink}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetEmbeddedObject(bool, byte[], string, bool, string, bool) {#setembeddedobject_1}

Définit les données de l'objet intégré.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label, bool updateIcon)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| linkToFile | Boolean | Indique si l'objet est lié au fichier. Si vrai, le paramètre objectData est ignoré. |
| objectData | Byte[] | Les données de l'objet intégré. |
| sourceFileName | String | Le nom du fichier. |
| displayAsIcon | Boolean | Indique si l'objet est affiché sous forme d'icône. Si vrai, les données d'image originales seront recouvertes par l'icône. |
| label | String | Le libellé de l'icône. Fonctionne uniquement lorsque displayAsIcon est vrai. |
| updateIcon | Boolean | Indique si l'icône est mise à jour automatiquement. |

### Remarques

Comme Aspose peut mettre à jour toutes les icônes de fichiers intégrés, il est préférable de pouvoir ajouter la bonne icône avec *updateIcon* à false.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un OleObject à la feuille de calcul
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Préparer les paramètres pour SetEmbeddedObject
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.docx");
                string sourceFileName = "sample.docx";
                bool displayAsIcon = true;
                string label = "Word Document";
                bool updateIcon = true;

                // Appeler SetEmbeddedObject avec les paramètres spécifiés
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label, updateIcon);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


