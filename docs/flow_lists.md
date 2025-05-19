### **任务列表**

任务列表展示了当前项目下已上线的任务的基本信息，包括任务名称、相关用户、调度状态、调度信息、所属基线、基线类型、血缘统计信息、最近执行时间、最近提交时间、任务标签信息及相关操作。

![](../attachments/202412/180d8cd562fb998a.png)

<table><tbody>
    <tr>

		<th bgcolor="#C0C0C0">**基本信息**</th>
		<th bgcolor="#C0C0C0">**说明**</th>
	</tr>
    <tr>

		<td bgcolor=white>任务名称</td>
		<td bgcolor=white>显示任务名称，如果当前任务调度已失效，则会在名称下面显示调度已过期失效。</td>
    </tr>
    <tr>

		<td bgcolor=white>相关用户</td>
		<td bgcolor=white>包括：负责人、创建人以及提交人。当只选择一个时，例如选择负责人，则此处只显示负责人。</td>
    </tr>
	<tr>

		<td bgcolor=white>调度状态</td>
		<td bgcolor=white>包括已调度和未调度。</td>
    </tr>
	<tr>

		<td bgcolor=white>调度信息</td>
		<td bgcolor=white>包括下次执行时间、首次执行时间、调度失效时间、调度周期、队列。</td>
    </tr>
	<tr>

		<td bgcolor=white>所属基线</td>
		<td bgcolor=white>显示当前任务挂载的基线信息，点击齿轮图标可进行“展示关联下游基线”设置，设置后列表中会展示任务关联下游所属的基线。![](/documents/uploads/projects/EasyDataBook/202302/17412c6e8b1111e9.png)</td>
    </tr>
	<tr>

		<td bgcolor=white>血缘统计信息</td>
		<td bgcolor=white>统计该任务的上下游任务数，包括全部上下游任务数、直接上下游任务数。其中全部上下游任务数后面括号内会显示总层数，若一个任务同时对应多层则按最大层数计数。</td>
    </tr>
	<tr>

		<td bgcolor=white>最近执行时间</td>
		<td bgcolor=white>任务最近一次执行时间。</td>
    </tr>

	<tr>
		<td bgcolor=white>最近提交时间</td>
		<td bgcolor=white>任务最近一次提交时间。</td>
    </tr>
	
	<tr>
		<td bgcolor=white>标签</td>
		<td bgcolor=white>任务支持打标签，可在表头设置中，查看已经设置的具体标签列。</td>
    </tr>

	<tr>
		<td bgcolor=white>操作</td>
		<td bgcolor=white>支持编辑、补数据、设置基线、设置优先级、暂停调度/恢复调度、取消调度、转交任务、血缘诊断、设置标签、修改调度生效时间等功能。</td>
    </tr>
</table>

点击某个任务前的![](/documents/uploads/projects/EasyDataBook/202204/16e34eaceb8f258c.png)图标可对当前任务进行展开，展开后显示节点列表，可了解各节点的**启用状态**、**节点类型**、**质量监控**配置情况以及**执行历史**。  
![](/documents/uploads/projects/EasyDataBook/202204/16e34ec5a163c038.png)  

在任务列表中，如果勾选了“展示关联下游基线”，则在任务列表筛选基线时，也会命中任务下游关联基线是所筛选基线的任务。例如，任务A的下游任务B所关联的基线是数仓8点基线，并且在任务列表中勾选了“展示关联下游基线”，此时在任务列表中筛选基线为“数仓8点基线”的任务，则会同时展示任务A与任务B，方便用户及时确认任务A的下游影响范围与重要性。