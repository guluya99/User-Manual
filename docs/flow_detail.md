[TOC]


在任务列表中点击某个任务可进入**任务详情**页面。

![](/documents/uploads/projects/EasyDataBook/202204/16e32bfff59ae09a.png)  

任务详情页上方提供了对任务操作的功能，包括**编辑**、**补数据**、**转交任务**、**设置基线**、**设置优先级**以及**取消调度**。  
![](/documents/uploads/projects/EasyDataBook/202204/16e32cda393a584e.png)  

- **编辑**：点击**编辑**按钮，会自动跳转至该任务的**离线开发**页面，方便使用人员对任务进行编辑。  
- **补数据**：点击**补数据**按钮，会在侧边弹出补数据的配置页面，可在此处进行单个任务的补数据操作，补数据的操作可参考[补数据实例运维](easytaskops_instance_ops_instance_complement.md)。  
![](/documents/uploads/projects/EasyDataBook/202204/16e32d82f4d637b9.png)  

- **转交任务**：点击**转交任务**按钮选择项目中成员，可变更任务负责人。  
![](/documents/uploads/projects/EasyDataBook/202204/16e32d9938ef7bec.png)  

- **设置基线**：点击**设置基线**按钮，可在弹框中设置已创建的基线，设置完成后任务会被挂载到这个基线上进行基线运维。  
![](/documents/uploads/projects/EasyDataBook/202204/16e32de09b595f17.png)  

- **设置优先级**：点击**设置优先级**按钮，可在弹框中设置**原始优先级**（原始优先级指的是任务本身的优先级，由于受任务依赖影响，优先级会从下游向上游传递升级，因此优先级存在变化情况）。  
![](/documents/uploads/projects/EasyDataBook/202204/16e32ec33ae782e5.png)  

- **取消调度**：具有**取消调度**权限的用户或是项目负责人、管理员、任务创建人员可点击**取消调度**按钮对任务进行取消调度操作。取消调度会将任务变成**未调度**状态，且后续不再生成调度实例，需谨慎操作。  
![](/documents/uploads/projects/EasyDataBook/202204/16e32f547243b015.png)  

#### **详细信息**

在**详细信息**页签主要展示任务的**基本信息**、**调度信息**以及**节点信息**。  

- **基础信息**：包括任务名称、提交人、任务类型、创建人、调度设置人以及最近修改时间信息。  
![](/documents/uploads/projects/EasyDataBook/202204/16e32fb9280d7862.png)  

- **调度信息**：包括最近执行时间、首次执行时间、下次执行时间、调度失效时间以及调度周期信息。  
![](/documents/uploads/projects/EasyDataBook/202204/16e32fc848daf575.png)  

- **节点信息**：包括该任务下包含的各节点状态、类型、是否配置质量监控以及查看节点功能。  
![](/documents/uploads/projects/EasyDataBook/202204/16e3306676114857.png)  
点击**查看节点**按钮，可查看节点的**SQL编辑器**及节点运行参数设置。  
![](/documents/uploads/projects/EasyDataBook/202204/16e331162ac376da.png)  

#### **任务血缘**

在**任务血缘**页签中展示当前任务的血缘情况。  
![](/documents/uploads/projects/EasyDataBook/202204/16e3310e87f403c1.png)  

血缘支持范围查看，如下：  

- 在范围处点击![](/documents/uploads/projects/EasyDataBook/202204/16e33124534c7037.png)按钮表示查看任务血缘的上下游。  
![](/documents/uploads/projects/EasyDataBook/202204/16e3312c59ef4d90.png)  

- 在范围处点击![](/documents/uploads/projects/EasyDataBook/202204/16e331319e816943.png)按钮表示查看任务血缘的上游。  
![](/documents/uploads/projects/EasyDataBook/202204/16e331356423fc9c.png)  

- 在范围处点击![](/documents/uploads/projects/EasyDataBook/202204/16e3313ac2226286.png)按钮表示查看任务血缘的下游。  
![](/documents/uploads/projects/EasyDataBook/202204/16e3317eb2e50a5e.png)  

**血缘层数**：表示当前任务的上下游层数，默认为**1**表示展示上下游各一层血缘。层数每+1，则上下游血缘分别多展示一层。例如此处设置层数为2，血缘展示如下：  
![](/documents/uploads/projects/EasyDataBook/202204/16e331ba2e9f94fa.png)  

当画布中显示的任务较多时，可在**搜索任务**框中输入任务名称进行任务的定位。  
![](/documents/uploads/projects/EasyDataBook/202204/16e33c06a35c6e54.png)  

点击任务节点，会在侧边弹出该节点详情，在详情中显示该任务节点的上下游全部任务层数，以及直接上下游任务数。在**基础信息**中，显示任务名称、所属项目以及负责人。在**调度信息**中，显示调度状态、调度周期、首次执行时间以及调度失效时间。  
![](/documents/uploads/projects/EasyDataBook/202204/16e34087440af633.png)  

点击任务名称可跳转对应的任务详情页面。   

#### **执行历史**

在**执行历史**页签中展示任务的**执行曲线**以及**执行历史**。  

**执行曲线**用来表示**线上调度**、**重跑**以及**补数据**的情况，横轴表示执行日期，纵轴表示执行时长，单位为s(秒)，支持展示近25次、近50以及近100次的执行情况。  
![](/documents/uploads/projects/EasyDataBook/202204/16e34408e8443c0c.png)  

**执行历史**已列表的形式展示当前任务产生的实例情况，包括**实例ID**、**状态**、**运行方式**、**计划执行时间**、**开始执行时间**、**结束时间**、**运行时长**以及**详情**。点击**详情**按钮可跳转至对应的**实例详情**页面。  
![](/documents/uploads/projects/EasyDataBook/202204/16e344698aa64834.png)  

#### **执行计划**

**执行计划**用来展示最近10条的线上调度和补数据执行计划。  
![](/documents/uploads/projects/EasyDataBook/202204/16e344ad24389c3f.png)  

点击实例中的**查看跨流依赖详情**，可查看**上游依赖详情**。页面中包括**任务依赖**和**节点依赖**信息，点击节点的**查看实例详情**按钮可跳转至实例详情页面，了解实例情况。  
![](/documents/uploads/projects/EasyDataBook/202204/16e344efa105c154.png)   

#### **基线信息**
在任务详情页面查看基线信息时，支持修改节点的平均运行时长，用于手动修正异常执行时长，以及查看下游所属基线（包括跨项目依赖），并查看下游任务列表，方便用户快速确认任务关联下游基线信息，并确认任务的优先级等重要性信息。   
![](../attachments/202311/1799e8d0e70fa687.png)