---
title: "Workbook.ImportXml"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Importe/Met à jour un fichier de données XML dans le classeur"
type: docs
url: /fr/net/aspose.cells/workbook/importxml/
---
## ImportXml(string, string, int, int) {#importxml_1}

Importe/Met à jour un fichier de données XML dans le classeur.

```csharp
public void ImportXml(string url, string sheetName, int row, int col)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| url | String | l'url/chemin du fichier xml. |
| sheetName | String | le nom de la feuille de destination. |
| ligne | Int32 | la ligne de destination |
| col | Int32 | la colonne de destination |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodImportXmlWithStringStringInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un objet classeur
            Workbook wb = new Workbook();
            
            // Importer les données XML dans la première feuille de calcul à partir de la cellule A1
            wb.ImportXml("data.xml", "Sheet1", 0, 0);
            
            // Enregistrez le classeur
            wb.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportXml(Stream, string, int, int) {#importxml}

Importe/Met à jour un fichier de données XML dans le classeur.

```csharp
public void ImportXml(Stream stream, string sheetName, int row, int col)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | le flux du fichier xml. |
| sheetName | String | le nom de la feuille de destination. |
| ligne | Int32 | la ligne de destination. |
| col | Int32 | la colonne de destination. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodImportXmlWithStreamStringInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer des données XML d'exemple
            string xmlData = @"<Products>
                <Product>
                    <Name>Laptop</Name>
                    <Price>999.99</Price>
                </Product>
                <Product>
                    <Name>Phone</Name>
                    <Price>699.99</Price>
                </Product>
            </Products>";

            // Convertir la chaîne XML en MemoryStream
            MemoryStream xmlStream = new MemoryStream();
            StreamWriter writer = new StreamWriter(xmlStream);
            writer.Write(xmlData);
            writer.Flush();
            xmlStream.Position = 0;

            try
            {
                // Importer les données XML dans le classeur à partir de la cellule A1 de la première feuille de calcul
                workbook.ImportXml(xmlStream, "Sheet1", 0, 0);

                // Enregistrez le classeur
                workbook.Save("ImportXmlDemo.xlsx");
                Console.WriteLine("XML data imported successfully to ImportXmlDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing XML: {ex.Message}");
            }
            finally
            {
                // Nettoyer les ressources
                xmlStream.Dispose();
            }
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


