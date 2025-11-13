---
title: Class GridJsOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.GridJs.GridJsOptions class. Represents all the load options for GridJs
type: docs
url: /net/aspose.cells.gridjs/gridjsoptions/
---
## GridJsOptions class

Represents all the load options for GridJs

```csharp
public class GridJsOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [GridJsOptions](gridjsoptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitrowsheightonload/) { get; set; } | Indicates whether to autofit rows height when loading the file,the default value is false. |
| [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/gridjsoptions/autooptimizeforlargecells/) { get; set; } | Gets/Sets whether to automatically optimize the load performance for worksheet with large cells. it will ignore some style /borders to reduce the load time. the default value is true. |
| [BaseRouteName](../../aspose.cells.gridjs/gridjsoptions/baseroutename/) { get; set; } | Gets/Sets the route URL base name for GridJs controller.the default is GridJs2 |
| [CustomPdfSaveOptions](../../aspose.cells.gridjs/gridjsoptions/custompdfsaveoptions/) { get; set; } | Gets/Sets the custom PdfSaveOptions for PDF export. If set, this will be used instead of the default options. the default value is null. |
| [EmptySheetMaxCol](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxcol/) { get; set; } | Gets/Sets default max column for an empty worksheet. the default value is 15. |
| [EmptySheetMaxRow](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxrow/) { get; set; } | Gets/Sets default max row for an empty worksheet. the default value is 12. |
| [FileCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/filecachedirectory/) { get; set; } | Gets/Sets the cache directory for storing spreadsheet file. We need to set it to a specific path before we use GridJs. |
| [FontFolders](../../aspose.cells.gridjs/gridjsoptions/fontfolders/) { get; set; } | Gets/Sets the fonts folders for fonts in the rendered pictures/shapes |
| [IgnoreEmptyContent](../../aspose.cells.gridjs/gridjsoptions/ignoreemptycontent/) { get; set; } | Gets/Sets whether to show the max range which includes data ,style, merged cells and shapes. if the last row or column contains cells with no value and formula but has custom style then we will not show this row/column when this vlaue is true。 the default value is true . |
| [IsCollaborative](../../aspose.cells.gridjs/gridjsoptions/iscollaborative/) { get; set; } | Gets/Sets whether to support collabrative editing,the default is false. |
| [IslimitShapeOrImage](../../aspose.cells.gridjs/gridjsoptions/islimitshapeorimage/) { get; set; } | Gets/Sets whether to limit the total display shape/image count in one worksheet ,if set to true, GridJs will limit the total count of the display shapes or images in one worksheet to MaxShapeOrImageCount the default value is true. |
| [LazyLoading](../../aspose.cells.gridjs/gridjsoptions/lazyloading/) { get; set; } | Gets/Sets whether to load active worksheet only,the default is false. |
| [MaxPdfSaveSeconds](../../aspose.cells.gridjs/gridjsoptions/maxpdfsaveseconds/) { get; set; } | Gets/Sets the max timed out seconds when save to PDF. the default value is 10. |
| [MaxShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagecount/) { get; set; } | Gets/Sets the total count of the display shapes or images in the active sheet,it takes effect when IslimitShapeOrImage=true. the default value is 100. |
| [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagewidthorheight/) { get; set; } | Gets/Sets the max width or height for a shape or an image ,GridJs will ignore the shape or image with the width or height larger than this, it takes effect when IslimitShapeOrImage=true. the default value is 10000. |
| [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxtotalshapeorimagecount/) { get; set; } | Gets/Sets the total count of the display shapes or images in the workbook,it takes effect when IslimitShapeOrImage=true. the default value is 300. |
| [MessageTopic](../../aspose.cells.gridjs/gridjsoptions/messagetopic/) { get; set; } | Gets/Sets the websocket destinations prefixed with "/topic". the default is "/topic/opr".used in collaborative mode only. |
| [PictureCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/picturecachedirectory/) { get; set; } | Gets/Sets the cache directory for pictures.(this takes effect when GridJsWorkbook.CacheImp is null) the default path will be "_piccache" inside the FileCacheDirectory. |
| [SameImageDetecting](../../aspose.cells.gridjs/gridjsoptions/sameimagedetecting/) { get; set; } | Gets/Sets whether to check if images have same source,the default is true the default value is true. |
| [SaveHtmlAsZip](../../aspose.cells.gridjs/gridjsoptions/savehtmlaszip/) { get; set; } | Gets/Sets whether to save html file as zip archive,the default is false. |
| [ShowChartSheet](../../aspose.cells.gridjs/gridjsoptions/showchartsheet/) { get; set; } | Gets/Sets whether to show chart worksheet. the default value is false . |
| [SkipInvisibleShapes](../../aspose.cells.gridjs/gridjsoptions/skipinvisibleshapes/) { get; set; } | Gets/Sets whether to skip shapes that are invisble to UI ,the default value is true. |
| [UsePrintArea](../../aspose.cells.gridjs/gridjsoptions/useprintarea/) { get; set; } | Gets/Sets whether to use PageSetup.PrintArea for the UI display range when the worksheet has PageSetup setting for PrintArea. the default value is false . |

## Fields

| Name | Description |
| --- | --- |
| [CacheImp](../../aspose.cells.gridjs/gridjsoptions/cacheimp/) | Custom implemention for cache storage,If you want to store cache in stream way ,you need to set and implement it. |

### See Also

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


