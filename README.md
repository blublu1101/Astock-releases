# Astock Releases

Astock (QMT Agent Desktop) 安装包发布仓库。

## 下载

访问 [Releases](https://github.com/blublu1101/Astock-releases/releases) 页面下载最新版本。

## 自动更新

应用内置自动更新功能，会自动检测并提示更新。

## 版本历史

- **v0.1.11**: Maintenance release
- **v0.1.7**: 大规模代码重构与功能增强
  - **IPC 模块化拆分**：主进程 IPC 拆分为 system / pi-agent / astock-api / settings / memory / notifications / skills / conversations / market / workspace 独立模块，新增模块注册表与测试
  - **Hooks 模块化拆分**：抽取 useChat（FE-01 会话-ID 守卫）、useNotifications / useAgentRuns / useHydration（FE-03 allSettled）、useConversations / useWorkspace / useMarket、useTheme / useSettings（无 Context）
  - **自动更新安全增强**：强化自动更新安全与配置校验；本地代码执行默认禁用并增加安全检查；补充 auto-updater 与 IPC 安全测试用例
  - **功能新增**：设置 UI 样式与启动自启设置管理、model gateway API 客户端、更新通知与记忆设置 UI、ConfirmDialog 组件增强、logo 更新、外部信息来源标注规则
  - **文档**：打包指南与代码执行策略文档更新；新增 god-object 重构计划、设计评审报告、用户指南、scroll-data-story 模板

- **v0.1.6**: 清理移除 autoSaveInterval 等冗余设置项

- **v0.1.5**: 修复Windows logo显示，添加自动更新功能

- **v0.1.4**: 初始版本
