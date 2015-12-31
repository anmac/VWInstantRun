## VWInstantRun

How many times you have to build and run your whole project when you just want to run 
a small piece of code to test a tiny doubt ?

Now with VWInstantRun, you won't run into this situation any more. An Xcode plugin let you build & run your selected lines of code in Xcode without running the whole project, you'll have the output instantly in your Xcode console.

![](run_swift_code_1.gif)
![](run_swift_code_2.gif)
![](run_swift_code_3.gif)

### Installation

Installation: You can clone or just download the project, then open project with Xcode, 
build and run project, and finally restart Xcode to active plugin.

### Alcatraz

Another way more easier option: This plugin can also be installed using [Alcatraz](https://github.com/alcatraz/alcatraz-packages). 
Just search for `VWInstantRun` in [Alcatraz](https://github.com/alcatraz/alcatraz-packages).

### Usage

Generally you just select your code in Xcode, then either use hotkey `⌘⌥⇧ + R` or go to `Product -> Instant Run` to 
build and run the lines of code selected. 

### Limitations

The purpose of this plugin is to run your code snippet instantly without building the whole project, so obviously it do have some limitations.

- The code selected should be isolated completely from other contexts (such as instance property, self, or there function, etc…), otherwise you will only have some compiler errors when you run that code snippet.
- Usually you need to add some stub values as input and add `print()` phrase to actually view your output in console view.
- For now, it only support Foundation module.

**This plugin certainly can not and should not replace your unit tests, at all. The suitable case is to test and prove some tiny doubts as I mentioned in blog.**

### Todo List
This plugin is still in a very early stage, here is a TODO list to show you a simple roadmap.
- [x] Swift code support.
- [ ] Objective-C code support. (In progress, should be done soon)
- [ ] More modules support.
- [ ] Run selected code with arguments inputed by user.

### More information
- You can checkout more implementation details in this [blog post](https://medium.com/@victor_wang/run-your-code-snippet-from-xcode-without-building-the-whole-project-1821cf85b2f2#.rkcfjqcl5).
- If you have __anything__ want to talk, feel free to raise an issue or say hello on Twitter to [@wangshengjia](https://twitter.com/wangshengjia), on Weibo to [@ShengjiaWang](http://www.weibo.com/1739447693/profile?topnav=1&wvr=6&is_all=1)

Enjoy :tada::tada:





###项目记录
1,项目是XCode插件,用于将选中行运行(有输出时可以在xcode命令行输出)
2,实现原理大概是将选中行写到一个swift文件中,并运行
3,为什么可以在xcode输出暂时不知道
4,项目中大量可以参考的函数




