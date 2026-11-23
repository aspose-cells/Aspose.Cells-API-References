---
title: "OdsCellField.FieldType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OdsCellField. Obtient et définit le type du champ"
type: docs
url: /fr/net/aspose.cells.ods/odscellfield/fieldtype/
---
## OdsCellField.FieldType property

Obtient et définit le type du champ.

```csharp
public OdsCellFieldType FieldType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyFieldTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des champs de cellule ODS avec différents types de champ et chaînes de format
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "Title Format");
            sheet.Cells.OdsCellFields.Add(1, 0, OdsCellFieldType.SheetName, "SheetName Format");

            // Démontrer l'utilisation de la propriété FieldType
            Console.WriteLine("Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);

            // Enregistrer et recharger pour démontrer la persistance
            workbook.Save("output.ods");
            workbook = new Workbook("output.ods");
            sheet = workbook.Worksheets[0];

            // Vérifier FieldType après rechargement
            Console.WriteLine("After reload - Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("After reload - Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);
        }
    }
}
```

### Voir aussi

* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


