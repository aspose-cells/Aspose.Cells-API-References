---
title: "OoxmlSaveOptions.EmbedOoxmlAsOleObject"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OoxmlSaveOptions. Indique s'il faut intégrer les fichiers Ooxml d'OleObject en tant qu'objet ole"
type: docs
url: /fr/net/aspose.cells/ooxmlsaveoptions/embedooxmlasoleobject/
---
## OoxmlSaveOptions.EmbedOoxmlAsOleObject property

Indique s'il faut incorporer les fichiers Ooxml d'OleObject en tant qu'objet ole.

```csharp
public bool EmbedOoxmlAsOleObject { get; set; }
```

### Remarques

Uniquement pour OleObject.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyEmbedOoxmlAsOleObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OLE Object Embedding");
            
            // Créer des options d'enregistrement OOXML et définir EmbedOoxmlAsOleObject
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.EmbedOoxmlAsOleObject = true;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx", saveOptions);
            
            Console.WriteLine("Workbook saved with OOXML embedded as OLE object.");
        }
    }
}
```

### Voir aussi

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


