<<<<<<< HEAD
# 天枢AutoOps运维管理系统

## 项目简介

天枢AutoOps运维管理系统(枢=枢纽+中心)是一个基于 Go + vue3 框架开发的企业级运维自动化平台，提供以下核心能力主机管理、配置中心、任务调度、K8s集群管理、监控告警等功能模块。统一平台，全栈治：打破 CI/CD、监控、CMDB、K8s、工单等系统孤岛，数据互通、策略统. 最终实现把常用的运维工具全部集成在一起，比如夜莺，jenkins，jumpserver，kuboard，cmdb，Archery，等等，实现运维自动化。
![alt text](assets/jg.png)

## 功能清单


| 功能模块 | 功能项 | 状态 |
|---------|--------|------|
| **CMDB资产管理** | 主机管理 | ✅ |
| | 主机管理-阿里-腾讯-百度-华为-跳板机 | ✅ |
| | 云密钥管理 | ✅ |
| | 主机终端管理 | ✅ |
| | 五类数据库管理(MySQL/PgSQL/Redis/ES/MongoDB) | ✅ |
| | windows 主机管理 | 🚧规划中 |
| | windows 远程桌面-guacamole | 🚧规划中 |
| | 交换机配置管理  | 🚧规划中 |
| **Kubernetes集群管理** | 多集群管理 | ✅ |
| | 节点管理 | ✅ |
| | Pod容器管理 | ✅ |
| | 容器配置-存储-配置-网络-路由管理 | ✅ |
| | K8s监控功能 | 🚧 规划中 |
| | K8s集群HPA自动扩缩容 | 🚧 规划中 |
| | K8s集群一键部署  | 🚧 规划中 |
| **服务管理** | 应用管理 | ✅ |
| | 应用快速发布-对接Jenkins可视化快速发布 | ✅ |
| | 应用工单上线流程发布 | ✅ |
| | 应用脚本上线工单 | ✅ |
| | 应用管理全局视图 | 🚧 开发中 |
| **监控中心** | 域名监控 | ✅ |
| | 主机基础资源监控 | ✅ |
| | 主机告警 | 🚧 开发中 |
| | 故障管理 | ✅ |
| | 数据库告警 | 🚧 开发中 |
| | 告警推送 | 🚧 开发中 |
| | 域名SSL证书申请 | 🚧 开发中 |
| **任务中心** | 定时任务 | ✅ |
| | 普通脚本任务(Shell/Python) | ✅ |
| | Ansible Playbook任务 | ✅ |
| **运维工具** | 常用运维资源安装 | ✅ |
| | Agent监控工具安装 | ✅ |
| **配置中心** | 主机凭据管理 | ✅ |
| | 通用资源账号管理 | ✅ |
| | 云资源密钥管理 | ✅ |
| **操作审计** | 登录日志审计 | ✅ |
| | 操作日志审计 | ✅ |
| | 数据库操作审计 | ✅ |
| | 终端录像审计 | 🚧 开发中 |
| **系统管理** | 用户管理 | ✅ |
| | 角色管理-RBAC授权 | ✅ |
| | 菜单管理-菜单-路由-按钮权限管理 | ✅ |
| | 部门管理 | ✅ |
| | LDAP认证集成管理 | ✅ |
| | 飞书-钉钉-微信-邮件集成 | 🚧 开发中 |
| **后续开发功能** | SQL工单系统 | 📋 规划中 |
| | 运维工单系统 | 📋 规划中 |
| | 运维全局巡检报告 | 📋 规划中 |
| | 优化运维仪表盘 | ✅ 完成 |
| | 运维知识库开发-Markdown写入-展示 | 📋 规划中 |
| | AI大模型分析功能 | 📋 规划中 |


### 优势对比

<details>
<summary><b>🔍 点击展开优势对比详情</b></summary>

#### DevOps运维管理系统优势
✅ **轻量级** - 单体应用，部署简单，资源占用少
✅ **全栈运维** - 同时管理传统主机和K8s集群，无需多套系统
✅ **开箱即用** - 内置CMDB、任务调度、SQL审计等企业级功能
✅ **二次开发友好** - Go语言，代码结构清晰，易于定制
✅ **成本低** - 无商业授权费用，适合中小企业
✅ **中文友好** - 国内开发，文档和支持更贴合国内使用习惯

## 核心竞争力分析
与传统运维平台相比，本系统在**自动化程度**、**一体化整合**、**可观测性**、**安全合规**、**扩展性与智能化演进**等维度展现显著优势：

---

### 1️⃣ 高度集成的一体化架构

| 对比维度 | 传统平台 | DevOps运维管理系统 |
|---------|---------|------------------|
| **系统构成** | 多个孤立工具拼凑（Zabbix + Ansible + CMDB） | 统一平台深度整合 |
| **数据流转** | 数据割裂，需手动同步 | 数据打通，实时联动 |
| **操作体验** | 多系统切换，操作繁琐 | 一个系统管全部，协同高效 |
| **核心价值** | ❌ 信息孤岛严重 | ✅ 消除信息孤岛，提升协同效率 |

---

### 2️⃣ 面向云原生的深度支持

| 对比维度 | 传统平台 | DevOps运维管理系统 |
|---------|---------|------------------|
| **技术栈** | 聚焦物理机/虚拟机 | 原生支持Kubernetes |
| **容器管理** | 支持薄弱或需插件 | 多集群管理、Pod/配置/网络/存储全要素管控 |
| **弹性伸缩** | 手动或简单脚本 | HPA自动扩缩容（规划中） |
| **核心价值** | ❌ 云原生支持不足 | ✅ 贴合现代微服务与容器化架构 |

---

### 3️⃣ 发布与工单流程深度融合

| 对比维度 | 传统平台 | DevOps运维管理系统 |
|---------|---------|------------------|
| **发布方式** | 手动脚本或简单CI | Jenkins可视化快速发布 |
| **变更管控** | 缺乏审批流程 | 工单审批流程 + 脚本上线工单 |
| **可追溯性** | 记录不完整 | 全流程可视化 + 操作审计 |
| **核心价值** | ❌ 审批、追溯能力弱 | ✅ 兼顾敏捷性与合规性 |

---

### 📊 总结对比

```
传统运维平台痛点：
├─ 🔴 工具碎片化 → 多系统切换，数据孤岛
├─ 🔴 流程不闭环 → 发布、审批、审计分离
├─ 🔴 云原生支持弱 → 难以适配容器化架构
└─ 🔴 智能化缺失 → 依赖人工经验判断

DevOps运维管理系统优势：
├─ 🟢 一体化设计 → 统一平台，数据打通
├─ 🟢 云原生原生支持 → K8s深度集成
├─ 🟢 合规审计 → 完整操作追溯
└─ 🟢 智能化演进 → AIOps技术前瞻性
```

> **💡 核心定位**：构建**高效、安全、可扩展且面向未来**的新一代智能运维中枢，远超传统运维平台的能力边界。

### 适用场景建议

| 场景 | 推荐方案 |
|------|---------|
| 中小企业混合环境（VM + K8s） | **DevOps运维管理系统** |
| 纯K8s环境，预算充足 | KubeSphere 或 Rancher |
| 多云多集群大规模部署 | Rancher |
| 国内企业，注重云原生完整性 | KubeSphere |
| 快速上线，资源有限 | **DevOps运维管理系统** |
| 需要传统运维+容器化双轨并行 | **DevOps运维管理系统** |

</details>

### 测试环境
http://autoops.com.cn/   
账号：test
密码：123456
### 视频安装使用介绍
https://www.bilibili.com/video/BV179Wxz1Ez6/?vd_source=37f81c1b36b3818cbad621bcbe5c3e49
![alt text](assets/b站.png)


## 安装步骤
docker一键安装

#### 拉取镜像(可选,首次部署会自动拉取)
```bash
docker pull crpi-aj3vgoxp9kzh2jx4.cn-hangzhou.personal.cr.aliyuncs.com/zhangfan_k8s/deviops-web:v5.0 
docker pull crpi-aj3vgoxp9kzh2jx4.cn-hangzhou.personal.cr.aliyuncs.com/zhangfan_k8s/deviops-api:v5.0 
docker pull crpi-aj3vgoxp9kzh2jx4.cn-hangzhou.personal.cr.aliyuncs.com/zhangfan_k8s/mysql:8.0.33 
docker pull crpi-aj3vgoxp9kzh2jx4.cn-hangzhou.personal.cr.aliyuncs.com/zhangfan_k8s/redis:6.2 
docker pull  crpi-aj3vgoxp9kzh2jx4.cn-hangzhou.personal.cr.aliyuncs.com/zhangfan_k8s/victoria-metrics:latest
docker pull crpi-aj3vgoxp9kzh2jx4.cn-hangzhou.personal.cr.aliyuncs.com/zhangfan_k8s/victoria-logs:latest 
docker pull crpi-aj3vgoxp9kzh2jx4.cn-hangzhou.personal.cr.aliyuncs.com/zhangfan_k8s/kafka:4.0.0    
docker pull crpi-aj3vgoxp9kzh2jx4.cn-hangzhou.personal.cr.aliyuncs.com/zhangfan_k8s/vector:latest-debian 
```

```bash
# 脚本+镜像版本+ip+前端端口
cd /root/deviops/docker
./devops-start.sh  v5.0   ip     8080
```


```bash
docker-compose up -d
### 2. 查看服务状态
docker-compose ps
### 3. 查看服务日志
docker-compose logs -f
### 4.访问服务
Web 前端: http://localhost:8080
默认账号: admin / 123456
```


## 感谢以下同学对本项目提供的打赏

<p align="center">
  <img src="assets/zanzhu/1.png" width="120" />
  <img src="assets/zanzhu/4.png" width="120" />
  <img src="assets/zanzhu/5.png" width="120" />
  <img src="assets/zanzhu/6.png" width="120" />
  <img src="assets/zanzhu/7.png" width="120" />
  <img src="assets/zanzhu/8.png" width="120" />
  <img src="assets/zanzhu/9.png" width="120" />
  <img src="assets/zanzhu/10.png" width="120" />
  <img src="assets/zanzhu/11.png" width="120" />
  <img src="assets/zanzhu/12.png" width="120" />
  <img src="assets/zanzhu/13.png" width="120" />
  <img src="assets/zanzhu/14.png" width="120" />
</p>

## 联系作者

## 技术交流+社区
- 微信技术交流: zf5391621
- 建议邮箱: zfwh1024@163.com
<img src="assets/zf.jpg" width="300" />

#### 加群技术交流
=======
# Autoops



## Getting started

To make it easy for you to get started with GitLab, here's a list of recommended next steps.

Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!

## Add your files

- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
- [ ] [Add files using the command line](https://docs.gitlab.com/topics/git/add_files/#add-files-to-a-git-repository) or push an existing Git repository with the following command:

```
cd existing_repo
git remote add origin http://172.30.1.101:8888/go/autoops.git
git branch -M main
git push -uf origin main
```

## Integrate with your tools

- [ ] [Set up project integrations](http://gitlab/go/autoops/-/settings/integrations)

## Collaborate with your team

- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
- [ ] [Set auto-merge](https://docs.gitlab.com/user/project/merge_requests/auto_merge/)

## Test and Deploy

Use the built-in continuous integration in GitLab.

- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/)
- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing (SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)

***

# Editing this README

When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thanks to [makeareadme.com](https://www.makeareadme.com/) for this template.

## Suggestions for a good README

Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.

## Name
Choose a self-explaining name for your project.

## Description
Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.

## Badges
On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.

## Visuals
Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.

## Installation
Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.

## Usage
Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.

## Support
Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.

## Roadmap
If you have ideas for releases in the future, it is a good idea to list them in the README.

## Contributing
State if you are open to contributions and what your requirements are for accepting them.

For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.

You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.

## Authors and acknowledgment
Show your appreciation to those who have contributed to the project.

## License
For open source projects, say how it is licensed.

## Project status
If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
>>>>>>> 47800ac4bad246ad4417a0a51f95722a83f8a580
