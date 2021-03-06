---
UID: NF:filterpipeline.IPrintPipelineFilter.ShutdownOperation
title: IPrintPipelineFilter::ShutdownOperation (filterpipeline.h)
description: The Pipeline Manager uses the ShutdownOperation method to shut down a filter if the print job is canceled or an error occurs.
old-location: print\iprintpipelinefilter_shutdownoperation.htm
tech.root: print
ms.date: 04/20/2018
keywords: ["IPrintPipelineFilter::ShutdownOperation"]
ms.keywords: IPrintPipelineFilter interface [Print Devices],ShutdownOperation method, IPrintPipelineFilter.ShutdownOperation, IPrintPipelineFilter::ShutdownOperation, ShutdownOperation, ShutdownOperation method [Print Devices], ShutdownOperation method [Print Devices],IPrintPipelineFilter interface, filterpipeline/IPrintPipelineFilter::ShutdownOperation, filterpipeline_5635f15b-3779-42ef-8b8d-3afeab1bab17.xml, print.iprintpipelinefilter_shutdownoperation
req.header: filterpipeline.h
req.include-header: 
req.target-type: Desktop
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Filterpipeline.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
targetos: Windows
req.typenames: 
f1_keywords:
 - IPrintPipelineFilter::ShutdownOperation
 - filterpipeline/IPrintPipelineFilter::ShutdownOperation
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Filterpipeline.h
api_name:
 - IPrintPipelineFilter.ShutdownOperation
---

# IPrintPipelineFilter::ShutdownOperation


## -description

The Pipeline Manager uses the <code>ShutdownOperation</code> method to shut down a filter if the print job is canceled or an error occurs.

## -returns

<code>ShutdownOperation</code> returns an <b>HRESULT</b> value.

## -remarks

The <code>ShutdownOperation</code> method is called by the pipeline manager if the job is canceled or an error occurs. Filters do not have to block this call until they completely finish using any resources. You should set up an internal state to indicate when filters need to cancel a job. Filters must call <a href="/windows-hardware/drivers/ddi/filterpipeline/nf-filterpipeline-iprintpipelinemanagercontrol-filterfinished">IPrintPipelineManagerControl::FilterFinished</a> when the filters are finished, which can be later.

## -see-also

<a href="/windows-hardware/drivers/ddi/filterpipeline/nn-filterpipeline-iprintpipelinefilter">IPrintPipelineFilter</a>



<a href="/windows-hardware/drivers/ddi/filterpipeline/nf-filterpipeline-iprintpipelinemanagercontrol-filterfinished">IPrintPipelineManagerControl::FilterFinished</a>
