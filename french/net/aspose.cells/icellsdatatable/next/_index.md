---
title: "ICellsDataTable.Next"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ICellsDataTable. Déplace le curseur d'une ligne vers le bas depuis sa position actuelle"
type: docs
url: /fr/net/aspose.cells/icellsdatatable/next/
---
## ICellsDataTable.Next method

Déplace le curseur d'une ligne vers le bas depuis sa position actuelle.

```csharp
public bool Next()
```

### Valeur de retour

si la nouvelle ligne courante est valide; false s'il n'y a plus de lignes

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTableMethodNextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            object[][] data = new object[][]
            {
                new object[] { "Name", "Age", "City" },
                new object[] { "John", 25, "New York" },
                new object[] { "Anna", 30, "London" },
                new object[] { "Peter", 35, "Paris" }
            };

            try
            {
                ImportTableOptions importOptions = new ImportTableOptions();
                importOptions.IsFieldNameShown = true;

                // Créer un ICellsDataTable à partir du tableau de données
                ICellsDataTable sourceDataTable = new CellsArrayDataTable(data, importOptions.IsFieldNameShown);

                // Importer le ICellsDataTable dans la feuille de calcul
                worksheet.Cells.ImportData(sourceDataTable, 0, 0, importOptions);

                ICellsDataTable dataTable = sourceDataTable;

                Console.WriteLine("Columns: " + string.Join(", ", dataTable.Columns));
                Console.WriteLine("Total Data Rows: " + (dataTable.Count == -1 ? "Unknown" : dataTable.Count.ToString()));

                dataTable.BeforeFirst();
                Console.WriteLine("\nData Table Contents:");

                while (dataTable.Next())
                {
                    Console.WriteLine($"{dataTable[0]}, {dataTable[1]}, {dataTable[2]}");
                }

                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Next method: {ex.Message}");
            }

            workbook.Save("MethodNextDemo.xlsx");
        }
    }

    // Implémentation personnalisée de ICellsDataTable pour les données de tableau
    internal class CellsArrayDataTable : ICellsDataTable
    {
        private readonly object[][] _data;
        private readonly bool _hasHeaders;
        private int _currentRow = -1;

        public CellsArrayDataTable(object[][] data, bool hasHeaders)
        {
            _data = data;
            _hasHeaders = hasHeaders;
        }

        public string[] Columns
        {
            get
            {
                if (_hasHeaders && _data.Length > 0)
                {
                    var headers = new string[_data[0].Length];
                    for (int i = 0; i < headers.Length; i++)
                        headers[i] = _data[0][i]?.ToString() ?? "";
                    return headers;
                }
                return new string[_data.Length > 0 ? _data[0].Length : 0];
            }
        }

        public int Count => _hasHeaders ? _data.Length - 1 : _data.Length;

        public object this[int column] => _data[_currentRow + (_hasHeaders ? 1 : 0)][column];

        public object this[string columnName]
        {
            get
            {
                int columnIndex = Array.IndexOf(Columns, columnName);
                if (columnIndex == -1)
                    throw new ArgumentException($"Column '{columnName}' not found.");
                return this[columnIndex];
            }
        }

        public void BeforeFirst()
        {
            _currentRow = -1;
        }

        public bool Next()
        {
            _currentRow++;
            return _currentRow < (_hasHeaders ? _data.Length - 1 : _data.Length);
        }
    }
}
```

### Voir aussi

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


