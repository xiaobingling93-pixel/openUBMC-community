# SIG 管理指南

### 申请新SIG流程

具体的申请流程如下：

1、使用SIG模板创建自己的新SIG

将 gitcode.com/openubmc/community Fork到你的GitCode下，利用SIG申请模板在sig目录创建你的sig文件夹，以及把SIG申请模板拷贝到该文件夹下。

~~~bash
git clone https://gitcode.com/${YOURGITCODE}/community

cd ./community/sig

cp -r sig-template sig-${YOURSIGNAME}

cd sig-${YOURSIGNAME}
~~~

2、完成新SIG README内容的填写

打开新创建sig目录下的README.md文件，按照推荐完成必选内容的填写

~~~bash
vi README.md
~~~

3、完成新SIG成员与SIG仓库的配置

请在sig-info.yaml文件中完成对SIG成员的配置

~~~bash
vi sig-info.yaml
~~~

4、提交PR

将以上修改提交到GitCode上，并在GitCode上创建一个Pull Request。

5、向TC发送邮件申请

给技术委员会发邮件（邮箱<tc@openubmc.org>），并在正文中包含主题“[新SIG提案]”和PR的链接

6、TC评审并反馈意见

技术委员会通常会在发送申请后的一周内反馈。如果遇到假期或重要会议等因素，可能会需要更长时间。在此期间，您可以进行任何有需要的更改

7、TC评审通过并合入

技术委员会将通过合并Pull Request的方式来批准您的申请。合入后社区基础设施团队会负责配置SIG相关角色与代码仓。