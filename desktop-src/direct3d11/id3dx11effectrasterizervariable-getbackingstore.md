---
title: ID3DX11EffectRasterizerVariable GetBackingStore method
description: Get a pointer to a variable that contains rasteriser state.
ms.assetid: 'aff62a6c-bdef-49ad-9492-5db0878f632e'
keywords: ["GetBackingStore method Direct3D 11", "GetBackingStore method Direct3D 11 , ID3DX11EffectRasterizerVariable interface", "ID3DX11EffectRasterizerVariable interface Direct3D 11 , GetBackingStore method"]
topic_type:
- apiref
api_name:
- ID3DX11EffectRasterizerVariable.GetBackingStore
api_location:
- N/A
- N/A.dll
api_type:
- COM
---

# ID3DX11EffectRasterizerVariable::GetBackingStore method

Get a pointer to a variable that contains rasteriser state.

## Syntax


```C++
HRESULT GetBackingStore(
  �UINT �����������������Index,
  �D3D11_RASTERIZER_DESC *pRasterizerDesc
);
```



## Parameters

<dl> <dt>

*Index* 
</dt> <dd>

Type: **[**UINT**](https://msdn.microsoft.com/library/windows/desktop/aa383751)**

Index into an array of rasteriser-state descriptions. If there is only one rasteriser variable in the effect, use 0.

</dd> <dt>

*pRasterizerDesc* 
</dt> <dd>

Type: **[**D3D11\_RASTERIZER\_DESC**](d3d11-rasterizer-desc.md)\***

A pointer to a rasteriser-state description (see [**D3D11\_RASTERIZER\_DESC**](d3d11-rasterizer-desc.md)).

</dd> </dl>

## Return value

Type: **[**HRESULT**](455d07e9-52c3-4efb-a9dc-2955cbfd38cc)**

Returns one of the following [Direct3D 11 Return Codes](d3d11-graphics-reference-returnvalues.md).

## Remarks

Effect variables are saved in memory in the backing store; when a technique is applied, the values in the backing store are copied to the device. Backing store data can used to recreate the variable when necessary.

> [!Note]  
> The DirectX SDK does not supply any compiled binaries for effects. You must use Effects 11 source to build your effects-type application. For more information about using Effects 11 source, see [Differences Between Effects 10 and Effects 11](d3d11-graphics-programming-guide-effects-differences.md).

�

## Requirements



|                    |                                                                                                                                              |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3dx11effect.h</dt> </dl>                                                    |
| Library<br/> | <dl> <dt>N/A (An Effects 11 library is available online as shared source.)</dt> </dl> |



## See also

<dl> <dt>

[ID3DX11EffectRasterizerVariable](id3dx11effectrasterizervariable.md)
</dt> </dl>

�

�




