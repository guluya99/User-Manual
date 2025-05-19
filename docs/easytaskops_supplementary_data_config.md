[TOC]

补数据配置管理当前支持**补数据时间窗口控制**、**补数据任务最大并发数上限**、**补数据审批控制**以及**补数据审批策略**的设置。项目负责人、管理员支持在该页面进行配置。   
![](/documents/uploads/projects/EasyDataBook/202302/17412bce74816777.png)   

<table><tbody>
    <tr>
		<th bgcolor="#C0C0C0">**配置项**</th>
		<th bgcolor="#C0C0C0">**描述**</th>
	</tr>
	<tr>
		<td bgcolor=white>补数据时间窗口</td>
		<td bgcolor=white>默认关闭。开启后，在指定时间范围内不允许补数据。</td>
    </tr>
    <tr>
		<td bgcolor=white>补数据任务最大并发数上限</td>
		<td bgcolor=white>最大并发数上限为100，支持设置1-100中任意整数。</td>
    </tr>
    <tr>
		<td bgcolor=white>补数据审批控制</td>
		<td bgcolor=white>默认关闭，开启后，补数据需要经过项目管理员审批才能创建补数据任务。（通过OpenAPI方式创建的补数据任务暂不支持审批控制）</td>
    </tr>
	<tr>
		<td bgcolor=white>补数据审批策略</td>
		<td bgcolor=white>审批策略支持**默认**和**自定义**两种，使用“默认”时，所有补数据任务都需经过项目管理员审批才能创建补数。自定义方式支持用户任意圈定任务范围，并配置一级审批人与二级审批人。</td>
    </tr>
</table>