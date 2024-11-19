# SIG组管理

## 背景

本目录下存放的是 openUBMC 社区中，所有代码仓与特别兴趣小组 （Special Interest Group，以下简称 SIG）的运作信息。

本目录下每一个子目录，代表一个 SIG。每个 SIG 的目录中，都会存在两个文件，分别是sig-info.yaml(保存SIG组信息)和repo-info.yaml（保存SIG组对应的Repo仓库信息）文件。所有被该 SIG 管理的代码仓，都以相应的独立 YAML 文件描述，存放于这两个文件中。


## 数据存放和管理方式

1. 每个 SIG 在 openubmc/community 仓的 sig 目录中各有一个独立的目录，目录下必须保存sig-info.yaml与 repo-info.yaml。
2. 原则上由 技术委员会 修改和维护。各个 SIG 所对应的 sig-info.yaml、repo-info.yaml 的修改，由各 SIG 的 maintainer 提交PR，经过技术委员会审视后合入。
4. 各 SIG 独立目录下的 README.md 为 SIG 的信息展示区。其中 SIG 基本信息需按模板留空，由工具自动填充。

## 格式规范

###  sig-info.yaml 文件格式

sig-info.yaml 文件为yaml格式承载，包含如下基本元素：
| 字段 | 类型 | 说明 |
|--|--|--|
| name | 字符串 | SIG组名称 |
| description | 字符串 | SIG组描述信息 |
| mailing_list | 字符串 | SIG组讨论邮件列表地址 |
| meeting_url | 字符串 | SIG例会纪要URL |
| maintainers | 列表   | SIG组所有maintainer名单   |
| committers | 列表 | SIG组所有committer名单    |
| repositories | 列表   | SIG组所管辖的GitCode仓库信息 |

注意：

1.maintainers 列表中每一条记录代表一位 maintainer 的个人信息， 每一条个人信息记录包含如下元素：

| 字段 | 类型 | 说明 |
|--|--|--|
| gitcode_id | 字符串 | GitCode ID, 必填 |
| name | 字符串 | 姓名(或者网名), 必填 |
| organization| 字符串 | 所在组织或单位, 选填 |
| email| 字符串 | 个人邮箱地址, 必填 |

2. committers的个人信息参考maintainers列表。
3. repositories 列表中每一条记录为SIG所管理的一组仓库信息：

| 字段 | 类型 |  说明 |
|--|--|--|
| repo | 字符串 | 一组SIG仓库 |


  4.maintainers和committers的职责划分
| 字段 | 类型 |  说明 |
|--|--|--|
|  | 字符串 | 仓库全名 |
| maintainers | 列表 | 主导代码合入的人员 |
| committers | 列表 | 参与代码审核的人员 |

### sig-info.yaml 文件样例
```
name: Infrastructure
description: The infrastructure team is responsible for system function development and maintenance of the openUBMC community.
created_on: '2024-12-31'
mailing_list: infra@openubmc.org
meeting_url: https://etherpad.openubmc.cn/p/infra-weekly-meeting-recaps
maintainers:
  - gitcode_id: georgecao
    name: George.Cao
    email: caozhi1214@qq.com
committers:
  - gitcode_id: weixin_43493709
    name: zhuchao
    email: tom_toworld@163.com
repositories:
  - openUBMC-test/infrastructure
  - openUBMC-test/openubmc-ci
```

### repo-info.yaml 文件格式

配置文件整体以yaml格式承载，包含如下基本元素：

| 名称 | 类型 | 说明 |
| :-- | :-- | :-- |
| name|字符串|仓库名称|
| description |字符串|仓库包含组件的描述|
| type|枚举类型，可选 public 或者 private | 仓库类型。private代码仓不提供开放访问|

### repo-info.yaml 文件样例
```
- name: infrastructure
  description: "Infrastructure repo is the warehouse operated and maintained by Infrastructure sig, including but not limited to CI access control, release platform, official website, etc."
  type: privacy
- name: openubmc-ci
  description: "The openubmc-ci repo is the repository for managing CI access control"
  type: privacy
- name: docs
  description: ""
  type: privacy
- name: website
  description: ""
  type: privacy
```
