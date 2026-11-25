---
title: "TableStyleCollection.GetBuiltinTableStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo TableStyleCollection. Ottiene lo stile di tabella predefinito"
type: docs
url: /it/net/aspose.cells.tables/tablestylecollection/getbuiltintablestyle/
---
## TableStyleCollection.GetBuiltinTableStyle method

Ottiene lo stile della tabella incorporato

```csharp
public TableStyle GetBuiltinTableStyle(TableStyleType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | TableStyleType | Il tipo di stile di tabella predefinito. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleCollectionMethodGetBuiltinTableStyleWithTableStyleTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per creare una tabella
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea una tabella
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[tableIndex];

            try
            {
                // Ottieni la raccolta di stili della tabella
                TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

                // Chiama GetBuiltinTableStyle con il parametro TableStyleType
                TableStyle builtinStyle = tableStyles.GetBuiltinTableStyle(TableStyleType.TableStyleMedium2);

                // Applica lo stile predefinito alla nostra tabella
                table.TableStyleName = builtinStyle.Name;

                Console.WriteLine($"Applied built-in table style: {builtinStyle.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBuiltinTableStyle method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("TableStyleCollectionMethodGetBuiltinTableStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TableStyle](../../tablestyle/)
* enum [TableStyleType](../../tablestyletype/)
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


