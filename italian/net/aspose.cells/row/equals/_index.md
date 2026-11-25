---
title: "Row.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Row. Verifica se questo oggetto si riferisce alla stessa riga di un altro"
type: docs
url: /it/net/aspose.cells/row/equals/
---
## Equals(object) {#equals_1}

Verifica se questo oggetto si riferisce alla stessa riga di un altro.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object | un altro oggetto |

### Valore di ritorno

true se due oggetti si riferiscono alla stessa riga.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea due righe da confrontare
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];
            
            // Imposta alcune proprietà per rendere le righe diverse
            row1.Height = 20;
            row2.Height = 25;
            
            try
            {
                // Chiama il metodo Equals con parametro Object
                bool result1 = row1.Equals((object)row2);
                Console.WriteLine($"Comparing row1 with row2: {result1}");
                
                // Confronta row1 con se stessa
                bool result2 = row1.Equals((object)row1);
                Console.WriteLine($"Comparing row1 with itself: {result2}");
                
                // Confronta con null
                bool result3 = row1.Equals((object)null);
                Console.WriteLine($"Comparing row1 with null: {result3}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
            
            workbook.Save("RowMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Row) {#equals}

Verifica se questo oggetto si riferisce alla stessa riga di un altro oggetto riga.

```csharp
public bool Equals(Row row)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Row | un altro oggetto riga |

### Valore di ritorno

vero se due oggetti riga si riferiscono alla stessa riga.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due righe da confrontare
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];

            // Imposta alcune proprietà per rendere le righe diverse
            row1.Height = 20;
            row2.Height = 25;
            row1.IsHidden = false;
            row2.IsHidden = true;

            try
            {
                // Chiama il metodo Equals per confrontare le righe
                bool areEqual = row1.Equals(row2);

                // Visualizza il risultato
                Console.WriteLine($"Are rows equal? {areEqual}");

                // Crea un'altra riga con le stesse proprietà di row1
                Row row3 = worksheet.Cells.Rows[2];
                row3.Height = row1.Height;
                row3.IsHidden = row1.IsHidden;

                // Confronta row1 con row3 (dovrebbe essere uguale)
                bool areEqual2 = row1.Equals(row3);
                Console.WriteLine($"Are rows equal after matching properties? {areEqual2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("RowEqualsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


