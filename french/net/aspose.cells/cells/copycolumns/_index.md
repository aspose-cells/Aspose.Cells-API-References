---
title: "Cells.CopyColumns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Copie les données et les formats d'une colonne entière"
type: docs
url: /fr/net/aspose.cells/cells/copycolumns/
---
## CopyColumns(Cells, int, int, int, PasteOptions) {#copycolumns_1}

Copie les données et les formats d'une colonne entière.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber, PasteOptions pasteOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | Cellules | L'objet Source Cells contient les données et les formats à copier. |
| sourceColumnIndex | Int32 | Indice de la colonne source. |
| destinationColumnIndex | Int32 | Indice de la colonne de destination. |
| columnNumber | Int32 | Le numéro de la colonne copiée. |
| pasteOptions | PasteOptions | les options de collage. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32PasteOptioDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // Créer un autre classeur comme destination
            Workbook destWorkbook = new Workbook();
            Worksheet destWorksheet = destWorkbook.Worksheets[0];

            // Copier les colonnes avec uniquement le formatage
            try
            {
                destWorksheet.Cells.CopyColumns(
                    worksheet.Cells, 
                    0, // source column index
                    0, // destination column index
                    2, // column count (copy 2 columns)
                    new PasteOptions() { PasteType = PasteType.Formats });
                
                Console.WriteLine("Columns copied successfully with formatting only.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error copying columns: " + ex.Message);
            }

            // Enregistrez le classeur
            workbook.Save("CopyColumnsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int) {#copycolumns}

Copie les données et les formats de colonnes entières.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | Cellules | L'objet Source Cells contient les données et les formats à copier. |
| sourceColumnIndex | Int32 | Indice de la colonne source. |
| destinationColumnIndex | Int32 | Indice de la colonne de destination. |
| columnNumber | Int32 | Le numéro de la colonne copiée. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajouter des données d'exemple aux colonnes
            cells["A1"].PutValue("Source1");
            cells["B1"].PutValue("Source2");
            cells["C1"].PutValue("Source3");
            cells["D1"].PutValue("Source4");
            cells["E1"].PutValue("Source5");

            // Copier les colonnes de l'index de colonne 1 (B) à l'index de colonne 3 (D), copier 1 colonne
            cells.CopyColumns(cells, 1, 3, 1);

            // Enregistrez le classeur
            wb.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int, int) {#copycolumns_2}

Copie les données et les formats de toutes les colonnes.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, 
    int destinationColumnIndex, int destinationTotalColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceCells | Cellules | L'objet Source Cells contient les données et les formats à copier. |
| sourceColumnIndex | Int32 | Indice de la colonne source. |
| sourceTotalColumns | Int32 | Le nombre de colonnes source. |
| destinationColumnIndex | Int32 | Indice de la colonne de destination. |
| destinationTotalColumns | Int32 | Le nombre de colonnes de destination. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Remplir les colonnes source (colonnes 0 et 1)
            cells[0, 0].Value = "Header 1";
            cells[0, 1].Value = "Header 2";
            for (int row = 1; row <= 4; row++)
            {
                cells[row, 0].Value = row * 100;
                cells[row, 1].Value = row * 200;
            }

            try
            {
                // Copier 2 colonnes de l'index 0 à l'index de destination 3, en insérant 2 colonnes
                cells.CopyColumns(cells, 0, 2, 3, 2);
                
                Console.WriteLine("Copied 2 source columns to destination position successfully");
                
                // Vérifier la copie en vérifiant les colonnes de destination (3 et 4)
                Console.WriteLine($"Destination column 3 value: {cells[0, 3].StringValue}");
                Console.WriteLine($"Destination column 4 value: {cells[0, 4].StringValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CopyColumns: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


