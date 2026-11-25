---
title: "AutoFilter.Custom"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AutoFilter. Filtra un elenco con un criterio personalizzato"
type: docs
url: /it/net/aspose.cells/autofilter/custom/
---
## Custom(int, FilterOperatorType, object) {#custom}

Filtra un elenco con un criterio personalizzato.

```csharp
public void Custom(int fieldIndex, FilterOperatorType operatorType1, object criteria1)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | Int32 | L'offset intero del campo su cui si desidera basare il filtro (da sinistra dell'elenco; il campo più a sinistra è il campo 0). |
| operatorType1 | FilterOperatorType | Il tipo di operatore del filtro |
| criteria1 | Object | Il criterio personalizzato |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alla colonna A (10 righe + intestazione)
            worksheet.Cells["A1"].PutValue("Numbers");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i); // A2-A11: 1-10
            }

            // Imposta l'intervallo dell'autofiltro (A1:A11)
            worksheet.AutoFilter.SetRange(0, 0, 0);

            try
            {
                // Applica filtro personalizzato: Numeri > 5
                worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterThan, 5);
                
                // Aggiorna il filtro per applicare le modifiche
                worksheet.AutoFilter.Refresh();
                
                Console.WriteLine("Custom filter applied: Column 0 values > 5");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Custom method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro filtrata
            workbook.Save("AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FilterOperatorType](../../filteroperatortype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Custom(int, FilterOperatorType, object, bool, FilterOperatorType, object) {#custom_1}

Filtra un elenco con criteri personalizzati.

```csharp
public void Custom(int fieldIndex, FilterOperatorType operatorType1, object criteria1, bool isAnd, 
    FilterOperatorType operatorType2, object criteria2)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | Int32 | L'offset intero del campo su cui si desidera basare il filtro (da sinistra dell'elenco; il campo più a sinistra è il campo 0). |
| operatorType1 | FilterOperatorType | Il tipo di operatore del filtro |
| criteria1 | Object | Il criterio personalizzato |
| isAnd | Booleano |  |
| operatorType2 | FilterOperatorType | Il tipo di operatore del filtro |
| criteria2 | Object | Il criterio personalizzato |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectBDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola dati di esempio
            worksheet.Cells["A1"].PutValue("Product ID");
            worksheet.Cells["A2"].PutValue(85);
            worksheet.Cells["A3"].PutValue(42);
            worksheet.Cells["A4"].PutValue(65);
            worksheet.Cells["A5"].PutValue(95);
            worksheet.Cells["A6"].PutValue(30);
            worksheet.Cells["A7"].PutValue(75);

            // Imposta l'intervallo dell'autofiltro (A1:A7)
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.SetRange(0, 0, 0); // Start row: 0 (A1), strartt column: 0 (A), end Column: 0 (A)

            try
            {
                // Applica filtro personalizzato: Maggiore o uguale a 50 E Minore o uguale a 100
                autoFilter.Custom(
                    0, // Field index (column A)
                    FilterOperatorType.GreaterOrEqual,
                    50, // First criteria
                    true, // AND combination
                    FilterOperatorType.LessOrEqual,
                    100 // Second criteria
                );

                Console.WriteLine("Custom filter applied successfully with parameters: " +
                    "(Int32, FilterOperatorType, Object, Boolean, FilterOperatorType, Object)");

                // Aggiorna i filtri e salva i risultati
                autoFilter.Refresh();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Custom method: {ex.Message}");
            }

            // Salva la cartella di lavoro filtrata
            workbook.Save("AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectBDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FilterOperatorType](../../filteroperatortype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


