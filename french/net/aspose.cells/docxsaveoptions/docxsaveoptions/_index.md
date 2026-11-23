---
title: "DocxSaveOptions.DocxSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur DocxSaveOptions. Représente les options d’enregistrement d’un fichier .docx"
type: docs
url: /fr/net/aspose.cells/docxsaveoptions/docxsaveoptions/
---
## DocxSaveOptions() {#constructor}

Représente les options d'enregistrement du fichier .docx.

```csharp
public DocxSaveOptions()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul et ajouter des données d’exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Initialiser DocxSaveOptions à l’aide du constructeur
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.SaveAsEditableShaps = true;
            
            // Enregistrer le classeur au format DOCX avec les options
            workbook.Save("output.docx", saveOptions);
            
            Console.WriteLine("Document saved successfully with DocxSaveOptions.");
        }
    }
}
```

### Voir aussi

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DocxSaveOptions(bool) {#constructor_1}

Représente les options d'enregistrement du fichier .docx.

```csharp
public DocxSaveOptions(bool saveAsImage)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| saveAsImage | Boolean | Si True, le classeur sera converti en quelques images du fichier .docx. Si False, le classeur sera converti en quelques tableaux du fichier .docx. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Enregistrer en DOCX avec les options par défaut
            workbook.Save("output_default.docx");
            
            // Enregistrer en DOCX avec DocxSaveOptions(true) - optimisé pour MS Word
            workbook.Save("output_optimized.docx", new DocxSaveOptions(true));
        }
    }
}
```

### Voir aussi

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


