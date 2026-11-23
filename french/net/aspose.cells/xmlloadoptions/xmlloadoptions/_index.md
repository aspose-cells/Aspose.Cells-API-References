---
title: "XmlLoadOptions.XmlLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur XmlLoadOptions. Représente les options de chargement du fichier xml"
type: docs
url: /fr/net/aspose.cells/xmlloadoptions/xmlloadoptions/
---
## XmlLoadOptions() {#constructor}

Représente les options de chargement du fichier xml.

```csharp
public XmlLoadOptions()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créez de nouvelles options de chargement XML
            XmlLoadOptions options = new XmlLoadOptions();
            
            // Définissez la conversion des valeurs numériques ou de date
            options.ConvertNumericOrDate = true;
            
            // Charger le classeur avec des options
            Workbook workbook = new Workbook("input.xml", options);
            
            // Accédez aux données de la cellule
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell Value: " + cell.Value);
            Console.WriteLine("Cell Type: " + cell.Type);
            
            // Enregistrer le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XmlLoadOptions(LoadFormat) {#constructor_1}

Représente les options de chargement du fichier xml.

```csharp
public XmlLoadOptions(LoadFormat type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | LoadFormat | Le type de format de chargement. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Créez une instance de XmlLoadOptions avec le paramètre LoadFormat
                LoadFormat loadFormat = LoadFormat.Xml;
                XmlLoadOptions xmlLoadOptions = new XmlLoadOptions(loadFormat);

                // Définissez certaines propriétés de XmlLoadOptions
                xmlLoadOptions.StartCell = "A1";
                xmlLoadOptions.IsXmlMap = true;
                xmlLoadOptions.ConvertNumericOrDate = true;

                // Créez un classeur en utilisant les options de chargement
                Workbook workbook = new Workbook("sample.xml", xmlLoadOptions);

                // Accéder à la première feuille de calcul
                Worksheet worksheet = workbook.Worksheets[0];

                // Affichez certaines informations
                Console.WriteLine("XML file loaded successfully with LoadFormat.Xml");
                Console.WriteLine($"First cell value: {worksheet.Cells["A1"].Value}");

                // Enregistrez le classeur
                workbook.Save("XmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XmlLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [LoadFormat](../../loadformat/)
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


