---
title: "ISmartMarkerCallBack.Process"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ISmartMarkerCallBack. Callback pour le traitement d'un smart marker"
type: docs
url: /fr/net/aspose.cells/ismartmarkercallback/process/
---
## ISmartMarkerCallBack.Process method

Rappel pour le traitement d'un smart marker.

```csharp
public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | L'index de la feuille. |
| rowIndex | Int32 | L'index de ligne. |
| colIndex | Int32 | L'index de colonne. |
| tableName | String | Le nom de la table du smartmarker. |
| columnName | String | Le nom de la table du smartmarker. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ISmartMarkerCallBackMethodProcessWithInt32Int32Int32StringStringDemo : ISmartMarkerCallBack
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ISmartMarkerCallBackMethodProcessWithInt32Int32Int32StringStringDemo callback = 
                new ISmartMarkerCallBackMethodProcessWithInt32Int32Int32StringStringDemo();

            try
            {
                // Appeler la méthode Process avec des paramètres d'exemple
                callback.Process(0, 5, 3, "Products", "ProductName");
                
                Console.WriteLine("Process method executed successfully with parameters (0, 5, 3, \"Products\", \"ProductName\")");
                
                // Définir une valeur pour afficher l'effet
                worksheet.Cells[5, 3].PutValue("ProcessedValue");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
            
            workbook.Save("ISmartMarkerCallBackProcessDemo.xlsx");
        }

        public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
        {
            // Implémentation de la méthode Process
            Console.WriteLine($"Processing - Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}, Table: {tableName}, ColumnName: {columnName}");
        }
    }
}
```

### Voir aussi

* interface [ISmartMarkerCallBack](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


