---
title: "Sınıf WebWorksheet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.Data.WebWorksheet class. Web bir çalışma sayfasını temsil eder."
type: docs
url: /tr/net/aspose.cells.gridweb.data/webworksheet/
---
## WebWorksheet class

Bir web çalışma sayfasını temsil eder.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet instead")]
public class WebWorksheet : Control, ISerializable
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WebWorksheet](webworksheet/#constructor)() | WebWorksheet'ın yapıcı metodu. |
| [WebWorksheet](webworksheet/#constructor_1)(MainWeb, GridWorksheet) | WebWorksheet'ın yapıcı metodu. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | Sütun koleksiyonunu bağlayın. |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | Çalışma zamanında aslında bağlanan veri kaynağı nesnesi. DataSource özelliği bir DataSet, DataTable veya DataView nesnesi olduğunda bu bir DataView nesnesidir. |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | Veri bağlama modunda, BindStartRow ve BindStartColumn, veri kaynağına bağlanacak ızgaranın konumunu gösterir. |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | Veri bağlama modunda, BindStartRow ve BindStartColumn, veri kaynağına bağlanacak ızgaranın konumunu gösterir. |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } |  |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | Alır [`WebCells`](../webcells/). |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } |  |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | Veri bağlama modunda bağlama satır sayısını alır. |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | Çok üyeli DataSource'dan DataMember'ı alır veya ayarlar. Genel olarak bir DataSet'in DataTable nesnesini temsil eder. |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | DataSource'u alır veya ayarlar. Genel olarak bir DataSet nesnesidir. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | Veri bağlama modunda, sayfada bağlama sütun başlığı başlıklarını oluşturup oluşturmayacağını gösterir. |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | HyperlinkCollection koleksiyonunu alır. |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | Çalışma sayfaları içinde kendisinin indeksini alır. |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | Çalışma sayfasının korumalı olup olmadığını alır veya ayarlar. Bir çalışma sayfası korunduğunda, IsLocked özelliği false olan hücre dışındaki tüm hücreler düzenlenemez. |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | Sayfanın adını alır veya ayarlar. |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } |  |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | Çalışma sayfasındaki veri doğrulama ayarları koleksiyonunu alır. |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | Bu sayfanın adının kontrolün sayfa sekmelerinde gösterilip gösterilmeyeceğini belirtir. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn)(int) | Sütun genişliğini otomatik olarak ayarlar. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Sütun genişliğini otomatik olarak ayarlar. Bu yöntem, sütundaki startRow'dan endRow'a kadar olan hücre aralığındaki içeriğe göre sütunu otomatik olarak ayarlar. AutoFitColumn kesin olmayan bir işlevdir. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | Yeni eklenen bağlama satırını iptal eder ve siler. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | Yeni eklenen bağlama satırını onaylar ve veri kaynağına ekler. |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | Başka bir çalışma sayfası nesnesinden kopyalar. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | Çalışma sayfası için bir veri kaynağı ayarladıktan sonra, bağlama sütunlarını otomatik olarak oluşturmak için bu yöntemi çağırın. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | Yeni bir bağlama satırı oluşturur ve veri kaynağına bağlar. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Sayfada ara toplam oluşturur. |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | Sayfayı DataSource'a bağla. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | Bir bağlama satırını siler. |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows)(int, int) | Satırları gruplar. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows_1)(int, int, bool) | Satırları gruplar. |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | Tüm hücreleri düzenlenebilir yapar. Bu, genişletilmiş bir özelliktir. |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | Tüm hücreleri yalnızca okunur yapar. Bu, genişletilmiş bir özelliktir; bu özelliğin gerçek hücrede korunamayacağını unutmayın, korumayı sürdürmek istiyorsanız lütfen setProtect kullanın. |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | Hücre aralığını düzenlenebilir yapar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Tüm hücreleri SetAllCellsReadonly yöntemiyle yalnızca okunur yapın. Ardından bu yöntemi, düzenlenebilir olacak hücre aralığını belirtmek için çağırın. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | Hücre aralığını yalnızca okunur yapar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Önce SetAllCellsEditable yöntemiyle tüm hücreleri düzenlenebilir yapın. Ardından bu yöntemi, yalnızca okunur olacak hücre aralığını belirtmek için çağırın. |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | Çalışma sayfasındaki bölmeleri dondurmayı kaldırır. |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | Satırların gruplamasını kaldırır. |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | Bağlama veri kaynağı kaydının özelliği değerini hücrenin değerine göre günceller. |

### Açıklamalar

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Lütfen bunun yerine GridWorksheet kullanın. Bu sınıf, Ağustos 2014'ten itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp

 [C#]
 ...
 using System.Web.UI.WebControls;
 ...
 ...

 WebWorksheets Worksheets = GridWeb1.WebWorksheets;
	WebCells cells = Worksheets[0].Cells;

	//Varsayılan satır yüksekliğini ayarlar
	cells.StandardHeight = new Unit(16, UnitType.Point);
	//Satır yüksekliğini ayarlar
	cells.SetRowHeight(2, new Unit(20, UnitType.Point));

	//Varsayılan sütun genişliğini ayarlar
	cells.StandardWidth = new Unit(50, UnitType.Point);
	//Sütun genişliğini ayarlar
	cells.SetColumnWidth(3, new Unit(80, UnitType.Point));

	//Hücreleri birleştir
	cells.Merge(5, 4, 2, 2);

	//Veri içe aktar
	DataSet1 ds1 = new DataSet1();

	for (int i =0; i<16; i++)
	{
		DataSet1.Table1Row row = ds1.Table1.NewTable1Row();
		row["c1"] = "hello1";
		row["c2"] = i;
		row["c3"] = "data";
		ds1.Table1.AddTable1Row(row);
	}

	GridWeb1.WebWorksheets.ImportDataView(ds1.Table1.DefaultView, null, null);

 //Excel dosyasından içe aktar
 Worksheets.ImportExcelFile("c:\\file1.xls");

 [Visual Basic]
	Imports System.Web.UI.WebControls
	...
	...

	Dim Worksheets As WebWorksheets =  GridWeb1.WebWorksheets
	Dim cells As WebCells =  Worksheets(0).Cells

	'Sets default row height
	cells.StandardHeight = New Unit(16, UnitType.Point)
	'Sets row height
	cells.SetRowHeight(2,New Unit(20,UnitType.Point))

	'Sets default colum width
	cells.StandardWidth = New Unit(50, UnitType.Point)
	'Sets column width
	cells.SetColumnWidth(3,New Unit(80,UnitType.Point))

	'Merge cells
	cells.Merge(5, 4, 2, 2)

	'Import data
	Dim ds1 As DataSet1 =  New DataSet1()

	Dim i As Integer
	For  i = 0 To 15
		Dim row As DataSet1.Table1Row =  ds1.Table1.NewTable1Row()
		row("c1") = "hello1"
		row("c2") = i
		row("c3") = "data"
		ds1.Table1.AddTable1Row(row)
	Next

	GridWeb1.WebWorksheets.ImportDataView(ds1.Table1.DefaultView, Nothing, Nothing)

	'Import from excel file
	Worksheets.ImportExcelFile("c:\\file1.xls")
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


