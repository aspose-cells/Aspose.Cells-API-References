---
title: "OleObjectCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode OleObjectCollection. Ajoute un OleObject à la collection"
type: docs
url: /fr/net/aspose.cells.drawing/oleobjectcollection/add/
---
## Add(int, int, int, int, byte[]) {#add}

Ajoute un OleObject à la collection.

```csharp
public int Add(int topRow, int leftColumn, int height, int width, byte[] imageData)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| hauteur | Int32 | Hauteur de oleObject, en unité de pixel. |
| largeur | Int32 | Largeur de oleObject, en unité de pixel. |
| imageData | Byte[] | Image de l'objet ole sous forme de tableau d'octets. |

### Valeur de retour

[`OleObject`](../../oleobject/) object index.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectCollectionMethodAddWithInt32Int32Int32Int32ByteDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparez les données de l'objet OLE (fichier Excel d'exemple sous forme de tableau d'octets)
            byte[] oleData;
            try
            {
                string sampleFilePath = "sample.xlsx";
                oleData = File.ReadAllBytes(sampleFilePath);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error reading sample file: {ex.Message}");
                return;
            }

            try
            {
                // Appelez la méthode Add avec les paramètres : (upperLeftRow, upperLeftColumn, height, width, imageData)
                int oleIndex = worksheet.OleObjects.Add(5, 2, 200, 300, oleData);

                Console.WriteLine($"OLE object added successfully at index: {oleIndex}");
                Console.WriteLine($"Position: Row 5, Column 2");
                Console.WriteLine($"Size: 200px height, 300px width");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("OleObjectAddDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int, int, byte[], string) {#add_1}

Ajoute un OleObject lié à la collection.

```csharp
public int Add(int topRow, int leftColumn, int height, int width, byte[] imageData, 
    string linkedFile)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| hauteur | Int32 | Hauteur de oleObject, en unité de pixel. |
| largeur | Int32 | Largeur de oleObject, en unité de pixel. |
| imageData | Byte[] | Image de l'objet ole sous forme de tableau d'octets. |
| linkedFile | String |  |

### Valeur de retour

[`OleObject`](../../oleobject/) object index.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class OleObjectCollectionMethodAddWithInt32Int32Int32Int32ByteStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparez les données de l'objet OLE
            int upperLeftRow = 1;
            int upperLeftColumn = 1;
            int height = 200;
            int width = 200;
            byte[] imageData = File.ReadAllBytes("sample.ole");
            string linkedFile = "sample.xlsx";

            try
            {
                // Appelez la méthode Add avec les types de paramètres spécifiques
                int index = worksheet.OleObjects.Add(upperLeftRow, upperLeftColumn, height, width, imageData, linkedFile);
                
                Console.WriteLine($"OLE object added at index: {index}");
                Console.WriteLine($"Total OLE objects in worksheet: {worksheet.OleObjects.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("OleObjectAddDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


