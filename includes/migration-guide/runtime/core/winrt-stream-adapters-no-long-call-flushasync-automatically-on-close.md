### <a name="winrt-stream-adapters-no-long-call-flushasync-automatically-on-close"></a><span data-ttu-id="bbf4d-101">WinRT 流适配器不再在关闭时自动调用 FlushAsync</span><span class="sxs-lookup"><span data-stu-id="bbf4d-101">WinRT stream adapters no long call FlushAsync automatically on close</span></span>

|   |   |
|---|---|
|<span data-ttu-id="bbf4d-102">详细信息</span><span class="sxs-lookup"><span data-stu-id="bbf4d-102">Details</span></span>|<span data-ttu-id="bbf4d-103">在 Windows 应用商店的应用中，Windows 运行时流适配器不再从 Dispose 方法调用 FlushAsync 方法。</span><span class="sxs-lookup"><span data-stu-id="bbf4d-103">In Windows Store apps, Windows Runtime stream adapters no longer call the FlushAsync method from the Dispose method.</span></span>|
|<span data-ttu-id="bbf4d-104">建议</span><span class="sxs-lookup"><span data-stu-id="bbf4d-104">Suggestion</span></span>|<span data-ttu-id="bbf4d-105">此更改应该为透明。</span><span class="sxs-lookup"><span data-stu-id="bbf4d-105">This change should be transparent.</span></span> <span data-ttu-id="bbf4d-106">开发人员可以通过编写如下代码还原之前的行为：</span><span class="sxs-lookup"><span data-stu-id="bbf4d-106">Developers can restore the previous behavior by writing code like this:</span></span><pre><code class="language-csharp">using (var stream = GetWindowsRuntimeStream() as Stream)&#13;&#10;{&#13;&#10;// do something&#13;&#10;await stream.FlushAsync();&#13;&#10;}&#13;&#10;</code></pre>|
|<span data-ttu-id="bbf4d-107">范围</span><span class="sxs-lookup"><span data-stu-id="bbf4d-107">Scope</span></span>|<span data-ttu-id="bbf4d-108">透明</span><span class="sxs-lookup"><span data-stu-id="bbf4d-108">Transparent</span></span>|
|<span data-ttu-id="bbf4d-109">版本</span><span class="sxs-lookup"><span data-stu-id="bbf4d-109">Version</span></span>|<span data-ttu-id="bbf4d-110">4.5.1</span><span class="sxs-lookup"><span data-stu-id="bbf4d-110">4.5.1</span></span>|
|<span data-ttu-id="bbf4d-111">类型</span><span class="sxs-lookup"><span data-stu-id="bbf4d-111">Type</span></span>|<span data-ttu-id="bbf4d-112">运行时</span><span class="sxs-lookup"><span data-stu-id="bbf4d-112">Runtime</span></span>|
