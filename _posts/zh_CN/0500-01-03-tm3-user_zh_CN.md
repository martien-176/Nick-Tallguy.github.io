---
layout: doc
title: Tasking Manager 3
permalink: /en/coordination/tasking-manager3/
lang: en
category: coordination
navigation: skip
---

# Tasking Manager 3


** 如果您使用的版本的用户界面与此处描述的用户界面不同，那么您应该查阅 [我们的版本概述](/en/coordination/tm-disambiguation)**

内容索引
-------------
-  [Quick Start Guide](/en/coordination/tasking-manager3/#quick-start-guide)  
-  [The Mapping Process](/en/coordination/tasking-manager3/#mapping-process)  
    -  [Logging in](/en/coordination/tasking-manager3/#tasking-manager-login)  
    -  [Options - language settings and user profile](/en/coordination/tasking-manager3/#options-amp-links)  
    -  [Finding a Project - list based and using a map view, searching and filtering](/en/coordination/tasking-manager3/#finding-a-project---tasking-manager-contribute-screen)  
    -  [Mapping a Task - select, work on and unlock a task](/en/coordination/tasking-manager3/#mapping-via-the-tasking-manager) 
-  [Getting Help - live and contacting the project administrator](/en/coordination/tasking-manager3/#getting-help)  
-  [Hints and Tips](/en/coordination/tasking-manager3/#editing-hints-and-tips)
-  [Validation](/en/coordination/tasking-manager3/#validation)

The [HOT OSM Tasking Manager](http://tasks.hotosm.org) is a tool that coordinates many people mapping a specific geographic area in OpenStreetMap.

OpenStreetMap 是一个多人协作的免费世界地图。任何人都可以向 OpenStreetMap 做贡献，以绘制世界上任何感兴趣的地方。 Tasking Manager只是一个向多人同时贡献 OpenStreetMap 地图的工具，同时对 OpenStreetMap 的大多数贡献都是由不使用 Tasking Manager的人完成的。

 Tasking Manager 3 是与 OpenStreetMap 主项目完全独立的工具。当你使用 Tasking Manager 3 向 OpenStreetMap 做贡献时，你实际上正在使用多种软件工具：

* OpenStreetMap-地理信息数据库
*  Tasking Manager-帮助协调在同一区域编辑 OpenStreetMap 数据的人员
* OpenStreetMap 编辑器- 将数据读取和写入 OpenStreetMap 数据库的软件

![TM overview][]

 Tasking Manager 3 的作用是将一个特定的地理区域分为多个称为 “Tasks” 的小区域，并在使用标准 OpenStreetMap 编辑器绘制时提供一种方法来 “检出（checkout）” 或 “锁定（lock）” 这些小区域之一。通过 “检出（checkout）” 或 “锁定（lock）” 其中一个小区域，你可以帮助确保没有其他人在同一区域进行绘制。当两个人在 OpenStreetMap 中完全相同的区域工作时，这有助于防止 “重复绘制” 或其他错误。

完成对该小区域的绘制后，您可以在Tasking Manager中记录您已完成该小区域的绘制，然后选择另一个 “任务（Task）” 进行绘制。


## 快速入门指南

1.如果您没有 OpenStreetMap 帐户，请转到 https://openstreetmap.org 并创建一个帐户。这将是您用来登录Tasking Manager的登录详细信息。<br/>
  ![TM Quick Start 1][]
2.访问 [http://tasks.hotosm.org/](http://tasks.hotosm.org/) 并通过右上角登录  
  ![TM Quick Start 2][]
  > 在开始绘制之前，您必须在个人资料中提供有效的电子邮件地址（可通过右上角菜单中的第一个条目访问）。
3.点击 “贡献” 并找到要处理的地图项目  
  ![TM Quick Start 3][]
4.阅读该项目的说明  
  ![TM Quick Start 4][]
5.点击 “地图” 选项栏  
  ![TM Quick Start 5][]
6.找到要处理的 “就绪（Ready）” 任务，点击它并选择 “开始测绘（Start Mapping）”  
  ![TM Quick Start 6][]
7.您将切换到 OpenStreetMap 编辑器，测绘说明中要求的所有功能。  
  ![TM Quick Start 7][]
8.完成测绘后，切换回Tasking Manager，然后单击 “标记为完成测绘（Mark as Completely Mapped）”（如果已完成），如果您只是出于某种原因需要停止测绘，则单击 “停止测绘（Stop Mapping）”。  
  ![TM Quick Start 8][]


## 测绘过程 

1.远程测绘人员在 OpenStreetMap 中创建一个帐户并登录Taskiing Manager 3。
1.测绘人员通常根据 Tasking Manager 项目经理设置的优先级和技能级别来查找要处理的项目。 
2.远程测绘人员选择任务方形，完成测绘，然后将任务标记为完成。
3.第二个远程测绘人员检查任务是否已完成到令人满意的水平，并将任务标记为 “已验证（validated）”
4.可以从项目的 “统计” 选项卡中监控项目测绘的进度，并且可以根据管理员的要求降级或归档项目。

### Tasking Manager 3 Login

Tasking Manager是一个单独的工具，用于协调 OpenStreetMap 中的测绘工作。但是，它利用了 OpenStreetMap 登录系统。这意味着您不需要创建单独的用户帐户即可使用任务管理器，但在使用任务管理器进行测绘之前，您确实需要创建 OpenStreetMap 帐户并登录 OpenStreetMap。

当你第一次访问Tasking Manager时，屏幕右上角会看到 “登录（Login）” 按钮。

![TM login 1][]

点击该按钮将带你进入 OpenStreetMap 网站。在那里，你必须登录并授予任务管理器对 OpenStreetMap 首选项的访问权限。如果您还没有帐户，请在 OpenStreetMap 网站上创建帐户。

![TM login 2][]

![TM login 3][]

登录 OpenStreetMap 后，您将返回到任务管理器。现在是将您的电子邮件地址添加到个人资料的时候了。点击右上角的用户名以打开菜单，然后选择第一个条目 “您的个人资料”。您可以使用表格右上角的相应按钮编辑联系人详细信息。Tasking Manager 允许发送消息，因此需要先提供有效的电子邮件地址，然后才能开始测绘。

单击贡献或入门将带您进入可以参与的项目列表。

### 选项和链接

Tasking Manager最初以英语显示-要更改为另一种语言，请单击窗口右上角的 ** 英语 **。

登录后，您可以点击顶部的用户名。在这里你可以：

-查看您的Tasking Manager个人资料，您可以在其中：
    -更新您的电子邮件地址和社交媒体账户
    -查看你的测绘经验级别
    -查看你参与的项目的列表和地图
-转到Tasking Manager中的 ** 消息 ** 屏幕（这与 OpenStreetMap 消息系统不同）
-注销

### 查找项目- Tasking Manager 3 贡献屏幕

单击主菜单栏中的 “贡献” 链接将带您进入Tasking Manager 中的项目主列表。

![TM contribute][]

Tasking Manager 贡献屏幕分为三个主要区域：

-左边的搜索和筛选选项
-项目列表
-项目列表的地图视图

#### 搜索和筛选选项

默认情况下，将显示所有可用于测绘的项目。您可以使用屏幕的 “高级搜索” 筛选器部分进一步缩小要处理的项目范围。

-项目编号-如果你知道要处理的项目编号，你可以在这里输入它并直接进入它。
-组织-这允许您只显示单个组织请求的项目。
-测绘困难度 - 有些项目比其他项目更难绘制。使用此选项，您可以找到最适合您的体验水平的项目。我们鼓励您处理最符合自己体验水平的项目，尤其是如果您是经验丰富的测绘人员。
-测绘类型- 这允许您查找包含要测绘的特定类型功能的项目。许多项目只关注一种类型的测绘，但项目可能包含多种类型的要素进行测绘。
-全文搜索-这允许您搜索项目描述中可能包含某个词或短语的项目。
-大型任务活动标签-项目可以有其他标签，表示较大的测绘活动项目是其中的一部分，您可以通过将这些标签输入到此字段中找到项目。

#### 地图视图
点击 “地图视图” 选项卡将显示一个地区中的项目数量。双击或放大将显示各个项目。放大后，地图上的点将进行颜色编码，红色是紧急的，黄色为高或中优先级，灰色为低优先级。单击地图上的任何点都将显示有关该项目的信息。点击项目标题将带您进入该项目。

![TM project map][]

### 通过Tasking Manager 3进行测绘

找到要处理的项目后，点击项目标题将带您进入该项目的详细条目。此详细视图包含：

-描述项目的重要性以及如何使用数据
-关于测绘工作的详细说明
-用于测绘工作审核的选择屏幕
-各个测绘任务区域的详细地图，以及有关其状态的信息。
-关于项目的问题或评论选项卡

![TM project description][]



#### 项目页

你需要了解的关于该项目的一切都在这里！顶部是测绘项目的完整描述以及有关该项目的信息。  

在描述下方，屏幕分为左侧和右侧部分。左侧部分是一个选项卡式面板，其中包含 “说明”、“地图”、“验证” 和 “问题和评论” 的选项卡。右侧是项目的地图以及要绘制的各项任务。

-未着色的任务已准备就绪并可以进行测绘
-粉红色的网格方块已被验证器宣布审核未通过，再次可用于测绘
-地图上的红色区域表示优先级较高的区域
-黄/金网格方块已完成第一次测绘并准备好进行验证
-蓝色任务目前正在进行
-深蓝色边框表示你选择的任务
-绿色任务已完成第二次映射，测绘工作已 “被审核”
-深灰色的任务已被测绘人员查看，标记为没有可接受的测绘影像 


#### 说明选项卡
这显示了测绘任务中所需的内容。项目存在难度范围，适合初学者、中级和高级测绘人员-这些说明将解释这一点。确保你阅读并理解本节。测绘项目有许多风格，用于许多不同的目的。一些常见的项目活动包括：  

- Road networks: Used by people on the ground to load data into hand held navigation tools, and to work out how to access remote areas  
- Mapping villages: Often used to identify places where people live and may be impacted  
- Mapping buildings: Used for damage assessments or contact tracing with diseases. Also used for population estimates.  
- Mapping rivers, walls and other features  

Not all areas of the world are similar to your own, so specific tagging advice may be provided. For example, Africa's road network is very different to typical American or European highway systems.  

There will be a section indicating the **Changeset comment** you should make sure appears in your editing programme when uploading/saving your changes, together with the **source** information you may (depending on your editing software) need to copy & paste to the source field on making changes.  

Sometimes, task specific imagery may be available - you may need to agree to a license in order to access it. Instructions usually will indicate the easiest way to load this into editors such as JOSM or iD.  

When checking a task marked as complete, validators will expect that the requirements from the instructions tab have all been completed. You may find completing an entire task is quite difficult - guidance below is available around unlocking tasks; as well as providing useful feedback for the next mapper.  

#### Activity and Stats button  

This tab contains statistics about the project. It is divided into two sections, a detailed list of the activity (formerly its own tab in the Tasking Manager 2.0) and summary section.

The summary contains a list of mappers who have completed at least one task within the project.  

A log of all the comments left on individual tasks is at the bottom of the page. These are comments left on tasks and should not be confused with the "Questions and Comments" tab which are general questions and comments about the overall project.

You can return to the main project contribution page by clicking on the project title on the Activity and Stats page.

#### Map Tab  

Click when you are ready to start mapping. You may choose an individual task to work on by selecting it from the map, or by clicking on the "Take a Task at random" option.  Only uncolored tasks can be selected in this tab or you will get a message saying the task can not be mapped. If you intend to validate, make sure you select the "Validate" tab.

![TM map tab][]

#### Selecting a task to map  

Having selected your task you will be able to see if there is any history for this task, such as a mapper starting to map, but realizing they do not have time to complete the task.  

Clicking on the **Start Mapping** button locks the task so that no other mapper can select it until it is released again, and starts a 2 hour (120 minute) countdown timer, at the end of which time the task is automatically released. It is good practice to check on your countdown timer on a regular basis - it is easy to become engrossed in your mapping and not realise your task has been released, and has now been selected by another mapper who has started mapping it too. This can lead to conflicts and problems.  


#### Editing choices

Different options for editing are presented to you as soon as you lock a task.

##### Edit with JOSM  

Start JOSM before using this link and it will automatically load the existing OSM data into JOSM.  

> 1.需要勾选 “开启远程控制”-在 ** 编辑/偏好设置/远程控制 ** 下
> 2.如果您之前安装过插件 “ContinosDownload”，最好将其禁用（在 JOSM 中的 ** 文件 ** 菜单下取消选中 “持续下载 OSM 数据”）。  
>  3. If JOSM does not load the imagery automatically as well, it can normally be found under the **Imagery** menu. [More info on imagery here ](/en/josm/more-about-josm/#add-imagery)  
  

##### iD editor  

选择此选项可自动启动 Web 浏览器的新选项卡或窗口，并加载现有 OSM 数据。Internet Explorer Web 浏览器目前不支持 ID而作为替换它将加载 Potlatch 2。带有任务管理器的原始选项卡或窗口仍然存在。  


##### Potlatch 2  

The editor will load in a new window or tab. Potlatch will not automatically display the task bounding box, but you can do so by following this procedure:  

1. In the Tasking Manager, select a task and click Start Mapping to lock it  
2.在 “Tasking Manager” 中，选择 “使用 JOSM 编辑”（如果窗口显示 “JOSM 远程控制没有响应...”，只需单击 “OK”）。  
3.在使用 JOSM 编辑按钮下方，文本会显示 “提示：下载以下 .gpx 文件...”。下载 .gpx 文件，然后记下它的保存位置。  
4.在Tasking Manager中，从使用 JOSM 编辑更改为使用 Potlatch 2 编辑。Potlatch 应该在新标签页中打开。  
5.在 Potlatch 中，选择背景，然后选择矢量文件...  
6.在加载矢量文件窗口中，在文件旁边的底部，单击打开，然后导航到刚下载的 .gpx 文件  
7.在加载矢量文件窗口中，确保 .gpx 文件的 “显示” 列中选中该选框，然后关闭窗口  
8.Potlatch 现在应该将边界显示为方形（可能是青色）。请注意，Potlatch 仍会在边界之外加载数据。  
  

##### Field Papers  

For use only when you are involved in a project where a local mapper has carried out a ground survey and marked a printed map with information such as road names. This map can be rescanned and used as a background image for a remote or local mapper to read the information and update the OpenStreeetMap data [Field papers section of LearnOSM](/en/mobile-mapping/field-papers/).  


#### Splitting a task square

Having selected your task and inspected it with the imagery in place, you may realise that there is far too much detail required for mapping. An example of this may be tracing buildings in dense urban areas, or locating small villages in large areas. As guidance, where it isn't possible for one person to complete within the 2 hour time limit you can often split the task into 4 smaller areas. *Use with caution* - if/when task squares are split too small it is difficult to judge what type of highway is involved, and to identify other features.  

> 请注意，关于先前已完成工作的其它有用评论将不再可用。


#### Unlocking a Task

![TM unlock][]

##### Unlocking a Task before it is complete

If you start working on a task, but cannot complete it for some reason, it is best practice to leave a comment against the task. Simply detail what remains and choose **Stop Mapping**. Make sure your comments are relevant and aimed to help out the next mapper.  

例如：  

    几乎完成，左上方的小村庄 
    in the task square to be traced though
  

##### Unlocking a Task that is completely mapped

It is very difficult to be completely certain that you have completed a task - however it is acceptable to mark the task as complete if you are fairly sure - the contents will be checked by another mapper when validating, and any small additions can be made then.  

For the process to work most effectively, mappers need to mark tasks as "Mapped" rather than leaving them for several other 'not sure' mappers to spend time also checking them.  

When you have finished editing and think that the task is complete, save any remaining edits with your editing programme, then return to the Tasking Manager.  

+ Add comments to the box detailing what you achieved and more importantly, what you are not certain of. For example; "Complete as far as I can see, but there is cloud covering the top right corner of the task & I cannot see to trace this area".  
+ Click on the "Mark as Completely Mapped" button, and your work is ready for review.  

##### Marking a Task as Bad Imagery

You will sometimes select a task that can not be mapped because the imagery is low resolution or has cloud cover. Just close that task in your editor and use the "Mark as Bad Imagery" button to record that the task can not be mapped due to poor imagery.


#### Sending a message from the comment box

When leaving a comment against a task, you can have the comment sent as a message to a named mapper. Much like Twitter, simply use an @ followed by the username. This will send a message to the user containing the comments from this box, plus a link to the task that the comments box relates to.  

例如：  

    @HOTMppr nice work tracing the building  
    details here. You missed a small group  
    of houses on the upper left of the task square,  
    I added a few in, but some still remain.  

这在验证或添加他人之前的工作时特别有用-您可以提供反馈，谢谢或更多。  

+ 你可能希望提供一个可能对测绘人员有帮助的网站的链接，例如 <http://learnosm.org/en/coordination/remote-tracing/#buildings-walls-compounds-barriers>  
+ Be aware that many people from around the world will be participating, so prefer simple, clear language. If you come across comments in other languages, tools such as Google Translate are reasonably effective.


#### Referring to a particular task when sending an email  

If you need to send a message, such as an email or an IRC message, and you are querying something concerning a particular task within a project (perhaps you need help identifying something from the satellite imagery):  

1. Click on the task square concerned  
2. Click on the address bar in your web browser, which should show something similar to 'http://tasks.hotosm.org/project/713?task=259'  
3. Copy this link into the message. 


## Getting help 

### E-Mail

For questions which might require a little research to answer or more detailed explanations, usually the best channel is to write to mapper-support@hotosm.org

### Live text based help

1. Sign up at slack.hotosm.org. This will require filling in a form and might take a while to be accepted.
2. Join the mapper-support channel

### Leaving a Project question / comment / contacting the Project creator

Using the "Comments" tab for the project you can see other users' questions and comments and leave one of your own. You can also click the "Contact Project Manager" link and that will automatically direct your comment/question to the project creator. 

All comments are public and it is not live chat. Use the Slack option above if you need immediate attention.

![TM comments][]


## Editing hints and tips  

到目前为止，您已经很好地了解Tasking Manager是什么，以及它支持的一些各种功能。与普通编辑不同，此工具通常用于有许多参与者的时间紧迫的项目-这可能与您习惯有些不同。  

Some general advice to heed when working in this tool:  

* Avoid mapping far outside of your task square - other mappers may be working in that area, resulting in duplicated efforts. It's OK to map objects such as buildings overlapping a boundary, but avoid going much further - upload immediately after mapping something at the border.  
* 将道路、溪流或其他特征稍微延伸到边界上-这样，下一个测绘人员就可以在您离开的位置选择，但在完成编辑后立即上传。  
* 如果您对特定功能是什么有疑问，请使用评论部分提出问题或查看 wiki。  
* 如果您犯了严重错误（例如，删除主要特征或关系），请使用 IRC 或评论框要求其他测绘人员帮助您恢复此错误。尝试包含变更集或对发生情况的描述。作为一项协作任务，许多其他测绘人员都在这里提供帮助-重要的是要记住每个人有时会犯错误。  
* 不要犹豫地询问反馈-验证你的工作的测绘人员可能很仅简短留言，但是如果他们知道与你可以进行对话，那么对所有参与者来说会好得多。用另一种语言进行交流可能很困难，当你必须翻译以及用不流利的语言传递信息时，很容易表达方式毕竟突兀。  
* 你不能审核自己的工作-第二只眼睛总是会保证更好的测绘质量。  
* 在其他测绘人员审核您的工作时，不要担心他们留言语气和风格，像您一样，他们只想确保所有数据都能准确。他们的反馈是关于剩余工作而不是对你迄今所做努力的批评。  


## Validation

Validation is the process of a second mapper reviewing the mapping of the initial mapper of a project task. It is designed to ensure complete, quality data and provide thanks, feedback and encouragment to mappers.

### Getting Started

Validation starts much the same way as mapping does, a volunteer finds a project they would like to work on, reads the instructions tab to be sure they understand what is called for and how it is expected to be mapped, but instead of selecting the mapping tab for the project, they select the "Validate" tab.

![TM select for validation][]

The validator can select a task by clicking on an individual task square, clicking "Select a random Task", select by user or draw a polygon to select multiple, connected tasks.

Unlike mappers, validators can select multiple tasks to perform validation on a larger scale than just one task.

### Selecting Multiple Tasks for Validation

New in the latest version of the Tasking Manager is the ability to select multiple tasks for validation, either by area or by user.

Depending on which editor you are using, this feature will behave differently.

In JOSM, a second OSM data layer will be created titled "Task Boundaries - Do Not Edit or Upload" and it will have uploading disabled in recent versions of JOSM. JOSM **will not download the OSM data** because it could be a very large amount of data. Instead the validator will have to use the task boundaries as a guide and download the data to the active editing layer manually.

#### Select by drawing a polygon

This option allows a validtor to draw a square around a group of tasks and check them all out at once.

Once in the editor of their choice, **the validator will have to manually download the OSM data** for task areas selected. This is to prevent downloading all of the OSM data between the selected Tasks.


#### Select By User

A list of mappers who have marked a task as done is presented. Hovering over anyone in the list will highlight the tasks they have marked as completed. The list also prensents three important pices of information about the mapper, their experience level, the number of days since they first started mapping using the Tasking Manager and the number of days since they last received feedback via validation. This allows the validator to specifically target new mappers, experienced mappers or mappers who have not had any feedback for an extended period of time.

Clicking on the "Start Validating" button will lock all the tasks completed by that mapper and allow the validator to open them in their editor of choice.

![TM multi selection][]

Once in the editor of their choice, **the validator will have to manually download the OSM data** for task areas selected. This is to prevent downloading all of the OSM data between the selected tasks.

### Finalizing Validation

Once the validator has finished the validation process either for one task or multiple tasks, they should return to the Tasking Manager and select one of the three choices that reflect the mapping of the task:

- Stop Validating - If you could not complete the validation process but must stop validating.
- Mark (all) as Valid - If the mapping is complete and accurate
- Mark (all) as Invalid - If the mapping is not complete or inaccurate.

For the last two choices the validator can and should leave a friendly, encouraging comment addressed to the mapper(s) involved and provide thanks for their contributions and feedback on their mapping. Please be considerate before marking a task as invalid. If just a few bits are missing add them yourself, explain what was missing in your comment but nevertheless mark the task as valid. New mappers will consider their completed task marked as invalid as a fairly harsh comment.




[TM overview]: /images/coordination/tasking_manager_overview.png
[TM Quick Start 1]: /images/coordination/tasking_manager_qs1.png
[TM Quick Start 2]: /images/coordination/tasking_manager_qs2.png
[TM Quick Start 3]: /images/coordination/tasking_manager_qs3.png
[TM Quick Start 4]: /images/coordination/tasking_manager_qs4.png
[TM Quick Start 5]: /images/coordination/tasking_manager_qs5.png
[TM Quick Start 6]: /images/coordination/tasking_manager_qs6.png
[TM Quick Start 7]: /images/coordination/tasking_manager_qs7.png
[TM Quick Start 8]: /images/coordination/tasking_manager_qs8.png
[TM login 1]: /images/coordination/tasking_manager_login1.png
[TM login 2]: /images/coordination/tasking_manager_login2.png
[TM login 3]: /images/coordination/tasking_manager_login3.png
[TM contribute]: /images/coordination/tasking_manager_contribute.png
[TM map tab]: /images/coordination/tasking_manager_map_tab.png
[TM unlock]: /images/coordination/tasking_manager_unlock_task.png
[TM project map]: /images/coordination/tasking_manager_project_map.png
[TM project description]: /images/coordination/tasking_manager_project_description.png
[TM comments]: /images/coordination/tasking_manager_comments.png
[TM task selection]: /images/coordination/tasking_manager_task_selection.png
[TM select for validation]: /images/coordination/tasking_manager_validation_selection.png
[TM multi selection]: /images/coordination/tasking_manager_multi_selection.png