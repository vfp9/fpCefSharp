# fpCefSharp

***翻译；xinjie  2021-01-15***

## 简介
使用 fpCefSharp，你可以为你的 Visual FoxPro 应用程序添加一个现代浏览器。它是CefSharp的一个封装，它使用.NET应用程序封装了CEF。要在一个表单中托管浏览器控件，你需要一个 fpDotNet 的实例。

更多的细节可以在我的[Virtual FoxFest 2020 白皮书](https://github.com/cwollenhaupt/fpCefSharp/blob/master/Demos/Files/Wollenhaupt_Browser.pdf) 和 [我的会议记录](https://www.youtube.com/watch?v=hf5pQKOb0n4)中找到。 

## 使用方法简介

从[最后释放的版本](https://github.com/cwollenhaupt/fpCefSharp/releases)下载 fpCefSharp ZIP 文件并解压。

fpDotNet文件夹包含一个你需要注册的COM控件。它包含一个CMD文件，你可以以管理员身份执行。你只需要这样做一次。与所有其他的COM控件一样，它在计算机上进行全局注册，可能会影响所有使用相同控件的应用程序。

prg文件可以被移到任意文件夹。演示文件可以从你的生成应用中删除。

ShowHtml.SCX是一个非常简单的模仿浏览器界面的控件的实现。你可以使用这个表单或以任何你想要的方式整合该控件。UI是COM对象。其他的都是由cefSharpBrowser类驱动的。

## 组件和依赖性
fpCefSharp 依赖于以下项目：

- [CefSharp](https://github.com/cefsharp/CefSharp)
- [wwDotNetBridge](https://github.com/RickStrahl/wwDotnetBridge)
- [fpDotNet](https://github.com/cwollenhaupt/fpDotNet)
