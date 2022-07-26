---
title: SetDataSource
second_title: Référence de l'API Aspose.Cells pour .NET
description: Définit la source de données dunICellsDataTableaspose.cells/icellsdatatable objet.
type: docs
weight: 120
url: /fr/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

Définit la source de données d'un[`ICellsDataTable`](../../icellsdatatable) objet.

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| dataSource | String | Le nom de la source de données. |
| cellsDataTable | ICellsDataTable | tableau de données. |

### Voir également

* interface [ICellsDataTable](../../icellsdatatable)
* class [WorkbookDesigner](../../workbookdesigner)
* espace de noms [Aspose.Cells](../../workbookdesigner)
* Assemblée [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

Définit la source de données d'un objet DataSet.

```csharp
public void SetDataSource(DataSet dataSet)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| dataSet | DataSet | Objet DataSet |

### Exemples

```csharp

[C#]

//Créez un objet de connexion, spécifiez les informations du fournisseur et définissez la source de données.
OleDbConnection con = new OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb");
//Ouvre l'objet de connexion.
con.Open();
//Créez un objet de commande et spécifiez la requête SQL.
OleDbCommand cmd = new OleDbCommand("Select * from [Order Details]", con);
//Crée un objet adaptateur de données.
OleDbDataAdapter da = new OleDbDataAdapter();
// Spécifiez la commande.
da.SelectCommand = cmd;
//Créer un objet de jeu de données.
DataSet ds = new DataSet();
//Remplit le jeu de données avec les enregistrements de la table.
da.Fill(ds, "Order Details");
// Crée une table de données par rapport à la table de l'ensemble de données.
DataTable dt = ds.Tables["Order Details"];
//Créer un objet WorkbookDesigner.
WorkbookDesigner wd = new WorkbookDesigner();
//Ouvre le fichier modèle (qui contient des marqueurs intelligents).
wd.Workbook = new Workbook("SmartMarker_Designer.xls");
// Définissez la table de données comme source de données.
wd.SetDataSource(dt);
//Traitez les marqueurs intelligents pour remplir les données dans les feuilles de calcul.
wd.Process(true);
// Enregistrez le fichier excel.
wd.Workbook.Save("outSmartMarker_Designer.xls");

[Visual Basic]

'Créez un objet de connexion, spécifiez les informations du fournisseur et définissez la source de données.
Dim con As OleDbConnection = New OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb")
'Ouvrez l'objet de connexion.
con.Open()
'Créez un objet de commande et spécifiez la requête SQL.
Dim cmd As OleDbCommand = New OleDbCommand("Select * from [Order Details]", con)
'Créez un objet adaptateur de données.
Dim da As OleDbDataAdapter = New OleDbDataAdapter()
'Spécifiez la commande.
da.SelectCommand = cmd
'Créez un objet de jeu de données.
Dim ds As DataSet = New DataSet()
'Remplissez le jeu de données avec les enregistrements de la table.
da.Fill(ds, "Order Details")
'Créer une table de données par rapport à la table de jeu de données.
Dim dt As DataTable = ds.Tables("Order Details")
'Créez un objet WorkbookDesigner.
Dim wd As WorkbookDesigner = New WorkbookDesigner()
'Ouvrez le fichier de modèle (qui contient des marqueurs intelligents).
Dim workbook As Workbook = New Workbook("SmartMarker_Designer.xls")
wd.Workbook = workbook
'Définissez la table de données comme source de données.
wd.SetDataSource(dt)
'Traitez les marqueurs intelligents pour remplir les données dans les feuilles de calcul.
wd.Process(True)
'Enregistrez le fichier excel.
wd.Workbook.Save("outSmartMarker_Designer.xls")
```

### Voir également

* class [WorkbookDesigner](../../workbookdesigner)
* espace de noms [Aspose.Cells](../../workbookdesigner)
* Assemblée [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

Définit la source de données d'un objet DataTable.

```csharp
public void SetDataSource(DataTable dataTable)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| dataTable | DataTable | Objet DataTableDataTable object |

### Voir également

* class [WorkbookDesigner](../../workbookdesigner)
* espace de noms [Aspose.Cells](../../workbookdesigner)
* Assemblée [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

Définit la source de données d'un objet DataView et le lie à un nom de source de données.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| dataSourceName | String | Nom de la source de données. |
| dataView | DataView | Objet DataView. |

### Voir également

* class [WorkbookDesigner](../../workbookdesigner)
* espace de noms [Aspose.Cells](../../workbookdesigner)
* Assemblée [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

Définit la source de données d'un objet DataView.

```csharp
public void SetDataSource(DataView dataView)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| dataView | DataView | Objet DataView |

### Voir également

* class [WorkbookDesigner](../../workbookdesigner)
* espace de noms [Aspose.Cells](../../workbookdesigner)
* Assemblée [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

Définit la source de données d'un objet IDataReader.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| name | String | Nom de la carte de la source de données. |
| dataReader | IDataReader | Objet IDataReaderIDataReader object |
| rowCount | Int32 | Le nombre de lignes de données. Si le marqueur intelligent ne contient pas "noadd", nous devons insérer des lignes par le nombre de lignes pour un problème de performances et des formules répétées dynamiques. -1 signifie que le paramètre est inutile. |

### Voir également

* class [WorkbookDesigner](../../workbookdesigner)
* espace de noms [Aspose.Cells](../../workbookdesigner)
* Assemblée [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

Définit la liaison de données à une variable.

```csharp
public void SetDataSource(string variable, object data)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| variable | String | Nom de variable créé à l'aide d'un marqueur intelligent. |
| data | Object | Données source. |

### Voir également

* class [WorkbookDesigner](../../workbookdesigner)
* espace de noms [Aspose.Cells](../../workbookdesigner)
* Assemblée [Aspose.Cells](../../../)

---

## SetDataSource(OleDbConnection) {#setdatasource_3}

Définit la source de données d'un objet OleDbConnection.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| connection | OleDbConnection | Objet OleDbConnectionOleDbConnection object |

### Voir également

* class [WorkbookDesigner](../../workbookdesigner)
* espace de noms [Aspose.Cells](../../workbookdesigner)
* Assemblée [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

Définit la source de données d'un objet SqlConnection.

```csharp
public void SetDataSource(SqlConnection connection)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| connection | SqlConnection | Objet SqlConnectionSQLConnection object |

### Voir également

* class [WorkbookDesigner](../../workbookdesigner)
* espace de noms [Aspose.Cells](../../workbookdesigner)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
