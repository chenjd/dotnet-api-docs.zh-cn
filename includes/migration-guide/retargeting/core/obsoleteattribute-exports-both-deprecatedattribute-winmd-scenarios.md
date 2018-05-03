### <a name="obsoleteattribute-exports-as-both-obsoleteattribute-and-deprecatedattribute-in-winmd-scenarios"></a><span data-ttu-id="8692c-101">ObsoleteAttribute 在 WinMD 方案中导出为 ObsoleteAttribute 和 DeprecatedAttribute</span><span class="sxs-lookup"><span data-stu-id="8692c-101">ObsoleteAttribute exports as both ObsoleteAttribute and DeprecatedAttribute in WinMD scenarios</span></span>

|   |   |
|---|---|
|<span data-ttu-id="8692c-102">详细信息</span><span class="sxs-lookup"><span data-stu-id="8692c-102">Details</span></span>|<span data-ttu-id="8692c-103">创建 Windows 元数据库（.winmd 文件）时，<xref:System.ObsoleteAttribute?displayProperty=name> 属性将导出为 <xref:System.ObsoleteAttribute?displayProperty=name> 和 [Windows.Foundation.DeprecatedAttribute](https://docs.microsoft.com/uwp/api/windows.foundation.metadata.deprecatedattribute)。</span><span class="sxs-lookup"><span data-stu-id="8692c-103">When you create a Windows Metadata library (.winmd file), the <xref:System.ObsoleteAttribute?displayProperty=name> attribute is exported as both <xref:System.ObsoleteAttribute?displayProperty=name> and [Windows.Foundation.DeprecatedAttribute](https://docs.microsoft.com/uwp/api/windows.foundation.metadata.deprecatedattribute).</span></span>|
|<span data-ttu-id="8692c-104">建议</span><span class="sxs-lookup"><span data-stu-id="8692c-104">Suggestion</span></span>|<span data-ttu-id="8692c-105">重新编译使用 <xref:System.ObsoleteAttribute?displayProperty=name> 属性的现有源代码可能会在从 C++/CX 或 JavaScript 使用该代码时生成警告。我们不建议将 <xref:System.ObsoleteAttribute?displayProperty=name> 和 [Windows.Foundation.DeprecatedAttribute](https://docs.microsoft.com/uwp/api/windows.foundation.metadata.deprecatedattribute) 同时用于托管程序集中的代码，这可能会导致生成警告。</span><span class="sxs-lookup"><span data-stu-id="8692c-105">Recompilation of existing source code that uses the <xref:System.ObsoleteAttribute?displayProperty=name> attribute may generate warnings when consuming that code from C++/CX or JavaScript.We do not recommend applying both <xref:System.ObsoleteAttribute?displayProperty=name> and [Windows.Foundation.DeprecatedAttribute](https://docs.microsoft.com/uwp/api/windows.foundation.metadata.deprecatedattribute) to code in managed assemblies; it may result in build warnings.</span></span>|
|<span data-ttu-id="8692c-106">范围</span><span class="sxs-lookup"><span data-stu-id="8692c-106">Scope</span></span>|<span data-ttu-id="8692c-107">边缘</span><span class="sxs-lookup"><span data-stu-id="8692c-107">Edge</span></span>|
|<span data-ttu-id="8692c-108">版本</span><span class="sxs-lookup"><span data-stu-id="8692c-108">Version</span></span>|<span data-ttu-id="8692c-109">4.5.1</span><span class="sxs-lookup"><span data-stu-id="8692c-109">4.5.1</span></span>|
|<span data-ttu-id="8692c-110">类型</span><span class="sxs-lookup"><span data-stu-id="8692c-110">Type</span></span>|<span data-ttu-id="8692c-111">重定目标</span><span class="sxs-lookup"><span data-stu-id="8692c-111">Retargeting</span></span>|
