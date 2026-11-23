---
title: "OdsSaveOptions.OdsSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur OdsSaveOptions. Crée les options d'enregistrement du fichier ods"
type: docs
url: /fr/net/aspose.cells/odssaveoptions/odssaveoptions/
---
## OdsSaveOptions() {#constructor}

Crée les options d’enregistrement du fichier ods.

```csharp
public OdsSaveOptions()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des cellules d'exemple avec différents styles de bordure
            worksheet.Cells["B2"].PutValue("Medium Border");
            worksheet.Cells["B4"].PutValue("Thick Border");
            worksheet.Cells["B7"].PutValue("Double Border");
            
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Medium;
            worksheet.Cells["B2"].SetStyle(style);
            
            style = workbook.CreateStyle();
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;
            worksheet.Cells["B4"].SetStyle(style);
            
            style = workbook.CreateStyle();
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
            worksheet.Cells["B7"].SetStyle(style);

            // Démontrer le constructeur OdsSaveOptions
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.GeneratorType = Aspose.Cells.Ods.OdsGeneratorType.LibreOffice;
            
            // Enregistrer en tant que fichier ODS
            workbook.Save("output.ods", saveOptions);
            
            Console.WriteLine("File saved with OdsSaveOptions constructor demo.");
        }
    }
}
```

### Voir aussi

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsSaveOptions(SaveFormat) {#constructor_1}

Crée les options d’enregistrement du fichier ods.

```csharp
public OdsSaveOptions(SaveFormat saveFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | Le format de fichier. Il doit être Ods, Ots, Fods ou Sxc, sinon le format enregistré sera automatiquement défini sur Ods. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue(123.45);
            
            try
            {
                // Appeler la méthode #ctor avec le paramètre SaveFormat
                OdsSaveOptions saveOptions = new OdsSaveOptions(SaveFormat.Ods);
                
                // Définir certaines propriétés des options d'enregistrement
                saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
                saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;
                
                Console.WriteLine("OdsSaveOptions constructor executed successfully with SaveFormat.Ods parameter");
                
                // Enregistrer le classeur avec les options spécifiées
                workbook.Save("OdsSaveOptionsCtorDemo.ods", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OdsSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [SaveFormat](../../saveformat/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


