---
title: "SvgImageOptions.setEmfRenderSetting"
linktitle: "setEmfRenderSetting"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Setting for rendering Emf metafile."
type: docs
weight: 540
url: /nodejs/aspose.cells/svgimageoptions/setemfrendersetting/
---

## setEmfRenderSetting()

Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When EmfRenderSetting.EMF_PLUS_PREFER is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is EmfRenderSetting.EMF_ONLY. For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.
