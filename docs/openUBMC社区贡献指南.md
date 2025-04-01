# open社区贡献指南

openUBMC是一款开源社区，完全依赖于社区提供友好的开发和协作环境。在参与社区贡献之前，请先阅读并遵守[openUBMC社区行为守则](./openUBMC社区行为准则.md)。

# 贡献步骤

## 步骤一：注册 GitCode 账号

* openUBMC使用GitCode作为代码托管仓：[https://gitcode.com/org/openUBMC](https://gitcode.com/org/openUBMC)

* 请参考[Gitcode用户指南](https://docs.gitcode.com/docs/users)注册GitCode账户，并在[用户设置](https://gitcode.com/setting/email)中设置您的主邮箱。

## 步骤二：签署 CLA

* 在参与社区贡献前，您还需要签署openUBMC社区贡献者许可协议（CLA）。

## 步骤三：找到您感兴趣的 SIG

* openUBMC社区内容按照不同的SIG来组织，以便于更好的管理和改善工作流程。openUBMC所有SIG组均是开放的，欢迎任何人来参与贡献。

### 因此，参与社区的正确方式：首先找到您感兴趣的SIG组。

* SIG的组织信息在openUBMC的SIG中心进行查看，也可以在[Community仓库](https://gitcode.com/openUBMC/community/tree/main/sigs)中查询。每个SIG组也会有各自的例会，SIG组例会是公开的，欢迎大家随时接入收听。

* 也欢迎通过[社区论坛](https://forum.openubmc.cn)、邮件的方式与SIG组的成员进行互动交流。

* 感兴趣的 SIG 组还未出现？新的 SIG 组等你来发起！欢迎发送申请邮件至：[tc@public.openubmc.cn](mailto:tc@public.openubmc.cn)，邮件申请模板请参考[申请流程](https://openubmc.cn/sig/apply)。

## 步骤四：开始您的贡献

社区的贡献不仅限于代码的开发，社区的每一个环节都欢迎大家进行贡献。

### 代码类贡献

每个SIG小组都会有各自规划的issue，您可以根据自己的兴趣挑选issue并解决它。

#### 给自己分配Issue

首先在评论框内输入 /assign，机器人就会将问题分配给您。 每个Issue下面可能已经有参与者的交流和讨论，如果您感兴趣，也可以在评论框中发表自己的意见参与Issue讨论。

#### 提交Issue

如果您准备向社区上报Bug或者提交需求，请在openUBMC社区对应的仓库上提交Issue。若不确定问题应提交到哪个仓库，请先在[社区论坛](https://forum.openubmc.cn)发帖咨询。

您也可以以[Issue](https://gitcode.com/org/openubmc/issues)的方式，或[社区论坛](https://forum.openubmc.cn)发起话题的方式提出自己的意见或建议。提交Issue请参考[Gitcode Issue提交指南](https://docs.gitcode.com/docs/repo/issues)。

#### 提交Pull Request

提交Pull Request请参考openUBMC社区Pull Request提交指南。 如果一次提交的代码量较大，建议将大型的内容分解成一系列逻辑上较小的内容，分段提交便于代码审查。

如果您的 Pull Request 没有引起足够的关注，可以通过对应 SIG 的邮件列表或者论坛上发帖进行求助。

#### 检视代码

openUBMC 作为一个开放的社区，我们希望所有参与社区的人都能成为活跃的检视者。 在进行代码审查时，可以参考[《The Gentle Art of Patch Review》（补丁审核的柔和艺术）](https://sage.thesharps.us/2014/09/01/the-gentle-art-of-patch-review/)这篇文章。文章中提出了一些关键的审查点，强调代码审查不仅能够帮助新贡献者更积极地参与进来，同时避免代码中出现细微的错误。在审查过程中，可以特别关注以下几个方面：

* **贡献的合理性：** 首先评估贡献者提出的想法是否合理，是否符合项目的目标和需求。

* **架构的准确性：** 检查贡献的代码是否遵循了正确的架构设计，是否与现有的代码库和设计原则相一致。

* **贡献的完整性：** 评估贡献的代码是否全面，是否包含了所有必要的功能和测试，以及是否考虑到了代码的可维护性和扩展性。

### 非代码类贡献

一个优秀的社区，不仅仅只是一些代码仓，而是拥有活跃的开发者在社区的各个角落持续的建设。非代码类的贡献包括但不限于以下的几个方式：

#### 文档建设

* 在阅读openUBMC社区文档时，若发现文档问题，请通过[提交issue](https://gitcode.com/openUBMC/docs/issues)的方式，或者[社区论坛发帖](https://forum.openubmc.cn/c/site-tc/41-category/41)的方式进行反馈。

* 有自己的见解？欢迎发表自己的文档。openUBMC社区有多种文档贡献方式，详情请参考[博客贡献指南](https://openubmc.cn/blog/contribution-guide)，或者通过邮件、论坛联系sig-docs小组。

#### 测试验证

* 希望加固社区的版本质量？请加入 [sig-QA](https://openubmc.cn/sig/QA)。

#### 其他工作

* 参与社区交流，通过[社区论坛](https://forum.openubmc.cn/)，帮助引导社区新人贡献社区，回答社区上的疑问等；

* 运维社区通信工具，包括协助 SIG 组的 Maintainer 完善 SIG 主页信息、组织社区例会等；

* 成为社区布道师，共同组织社区聚会，包括 Meetups、直播、社区开发者大会等；

* 参与社区宣传推广与内容制作，事件/技术/课程/视频请投稿至[TC](mailto:tc@public.openubmc.cn)；

* 参与社区基础设施建设，请加入 [sig-infrastructure](https://openubmc.cn/sig/infrastructure)

* 参与社区视觉设计，请联系[TC](https://openubmc.cn/sig/TC)

* 参与社区翻译服务，请联系 [TC](https://openubmc.cn/sig/TC)

## 步骤五：与社区一起成长

* 我们欢迎所有人参与 openUBMC 社区贡献，我们的目标是发展一个由贡献者组成的活跃、健康的社区。关于 Maintainer、Committer 等社区角色，请参考[SIG中心](https://openubmc.cn/sig)。