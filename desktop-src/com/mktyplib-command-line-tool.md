---
title: MkTypLib Command-Line Tool
description: MkTypLib is a command-line application that processes an IDL file to produce a type library. It can also be used to generate a C or C++ header file.
ms.assetid: '883d380d-1d73-439b-9f11-ee89fc62fdfd'
---

# MkTypLib Command-Line Tool

\[The Mktyplib.exe tool is obsolete. Use the MIDL compiler instead. If you need backward compatibility with old Automation programs, use the MIDL compiler with the **/mktyplib203** option.\]

MkTypLib is a command-line application that processes an IDL file to produce a type library. It can also be used to generate a C or C++ header file.

To generate a type library from a ODL file:

-   From the command prompt, run the following command:

    **mktyplibÂ ***filename*

    where *filename*is the name of the ODL file.

MkTypLib also supports several optional parameters. For a complete list, run the following command line:

**mktyplib /?**

Because MkTypLib is an obsolete application, it cannot parse IDL files or files with interfaces defined outside of a [**library**](https://msdn.microsoft.com/library/windows/desktop/aa367069) statement. For more information, see [Differences Between MIDL and MkTypLib](https://msdn.microsoft.com/library/windows/desktop/aa366797).

## Related topics

<dl> <dt>

[Translating to C++](translating-to-c--.md)
</dt> </dl>

 

 



