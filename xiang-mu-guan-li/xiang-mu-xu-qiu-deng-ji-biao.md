# 2.1 项目档案（业务类）

## 1. 基础信息操作

### 1.1  权限

登录者能看到：是制单人或业务员、有该单据的审批权限、在该单据的项目成员列表中的所有单据。

### 1.2   新增

点击新增跳转到新增界面。

1） 红色星号（\*）表示必填。

2） 项目号系统自动生成，规则：NE-区域缩写-年月日+两位流水号，例：2018/09/21华东地区第一个项目的项目号为：NE-HD-2018092101

3） 业务类的项目状态默认为未签约，是否终端客户默认为是。

4） 要求完成日期必须大于等于提出需求日期。

5） 计划完成日期必须大于等于计划开始日期

6） 制单人系统自动填写，即当前登录者，业务员默认为制单人，可修改。

4）  填完相关信息后，可点击【**暂存**】或 【**提交**】。点击**暂存**：只保存数据，制单人或业务员可再次修改。

点击**提交**按钮：保存数据后会创建一个审批流，审批流产生后，不能再修改数据，如图所示。

![](../.gitbook/assets/image%20%28106%29.png)

### 1.3   修改

1） 只有未产生审批流的单据可以修改，存在审批流的单据不支持修改（处理中、已完结、已关闭），如图所示。

![](../.gitbook/assets/image%20%2896%29.png)

2）只有研发经理审批过的单据才能被合同档案或项目进度计划引用。

### 1.4 删除

1）只能删除未产生审批流或已关闭的单据。

2）存在审批流或已被合同档案或项目进度计划引用的单据均不能删除，如图所示。

![](../.gitbook/assets/image%20%2816%29.png)

![](../.gitbook/assets/image%20%2812%29.png)

3）若想删除有审批流的单据，需先关闭单据（只有制单人或业务员才有权限作关闭单据，关闭单据：项目状态为已关闭，流程状态为已关闭）如图所示。

![](../.gitbook/assets/image%20%2851%29.png)

### 1.5  关闭

1）只有该单据的制单人或业务员才有关闭权限，注：关闭后的单据，项目状态为已关闭，流程为已关闭，关闭后的单据只供查询或删除，不能再做任何修改操作。

2）被项目进度计划引用的单据，需先关闭项目进度计划，才能执行关闭操作。

### 1.6 调整项目计划日期

1）只有已完结的单据才能调整项目计划日期。

2）只有该单据的项目经理或项目工程师才有权限调整项目计划日期。

### 1.7  查询

可根据项目号，客户名称，项目状态，潜在竞争对手，是否终端客户，区域，业务员（工号和姓名均可）进行查询，如图所示。

![](../.gitbook/assets/image%20%2828%29.png)

###  

## 2. 流程

### 2.1  审批流

![](../.gitbook/assets/image%20%287%29.png)



1）  制单人提交后业务自动审批通过，流转到项目经理节点。 

2） 项目经理节点：项目经理评估后选拒绝或同意，默认为同意，若选拒绝，需备注拒绝理由，流程直接结束，若选同意，则需指派项目工程师及选择研发总监，项目工程师节点自动审批通过，流程直接流转到研发总监节点。如图所示。

![](../.gitbook/assets/image%20%284%29.png)

![](../.gitbook/assets/image%20%2858%29.png)

3）  研发总监节点：研发总监有拒绝权限，若选拒绝，则需备注拒绝理由，流程直接结束，若选同意，则需指派研发经理，后流转到研发经理节点。

![](../.gitbook/assets/image%20%282%29.png)

![](../.gitbook/assets/image%20%2899%29.png)

4）  研发经理节点：研发经理需指派研发工程师，可同时指派多个，范围（只能选择该研发总监管理的部门成员），后流转到指定的研发工程师处，如图所示。

![](../.gitbook/assets/image%20%2850%29.png)

![](../.gitbook/assets/image%20%28118%29.png)

5） 研发工程师确认：当该流程中的所有研发工程师均确认完毕后，流程结束，如图所示。

![](../.gitbook/assets/image%20%2876%29.png)

### 2.2 流程信息查看

可以查看某个审批流的所有流转信息，如图所示。

![](../.gitbook/assets/image%20%2856%29.png)

### 2.3   项目成员

1） 只有在项目管理成员角色中的人员才可以设置项目成员。当项目经理节点同意通过后，系统自动插入项目负责人（即项目工程师）、项目经理、研发总监，如图所示。

2） 添加、删除、插入。点击删除将会删除选中的数据，点击插入如有选中的成员，则会在该选中的成员前插入一行数据，若没有，则在最后追加一行。

![](../.gitbook/assets/image%20%2887%29.png)

### 2.4   合同联络函

只有在项目管理成员角色中的人员才可以上传，上传后，即可点击通知邮件发送给相关人员，点击邮件通知后，可以选择发送或全部发送或发送未发送成员。如图所示。

![](../.gitbook/assets/image%20%28101%29.png)

![](../.gitbook/assets/image%20%28104%29.png)

### 2.5  方案文件

只有被项目计划关联且研发经理同意后的文件才能被看到。

![](../.gitbook/assets/image%20%28111%29.png)

![](../.gitbook/assets/image%20%2862%29.png)

![](../.gitbook/assets/image%20%28108%29.png)





