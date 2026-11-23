---
title: "ListObject.PutCellFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ListObject. Met la formule dans la cellule du tableau"
type: docs
url: /fr/net/aspose.cells.tables/listobject/putcellformula/
---
## PutCellFormula(int, int, string) {#putcellformula}

Placez la formule dans la cellule du tableau.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | Le décalage de ligne dans le tableau. |
| columnOffset | Int32 | Le décalage de colonne dans le tableau. |
| formule | String | La formule de la cellule. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Ajoutez des données d'exemple pour créer une table
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["C1"].PutValue("Formula");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue(20);

            // Créer un objet liste (table)
            int index = sheet.ListObjects.Add("A1", "C3", true);
            ListObject table = sheet.ListObjects[index];

            // Ajouter une nouvelle ligne et définir les valeurs/la formule
            table.PutCellValue(4, 0, 3); // Row 4, Column 0 (ID)
            table.PutCellValue(4, 1, 30); // Row 4, Column 1 (Value)
            table.PutCellFormula(4, 2, "=B3*2"); // Row 4, Column 2 (Formula)

            // Enregistrez le classeur
            wb.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellFormula(int, int, string, bool) {#putcellformula_1}

Placez la formule dans la cellule du tableau.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula, bool isTotalsRowFormula)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | Le décalage de ligne dans le tableau. |
| columnOffset | Int32 | Le décalage de colonne dans le tableau. |
| formule | String | La formule de la cellule. |
| isTotalsRowFormula | Boolean |  |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple pour créer un objet de liste
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            
            // Créer un objet de liste
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Démontrer PutCellFormula
            listObject.PutCellFormula(3, 0, "=SUM(A2:A3)", true);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


