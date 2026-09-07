# IPZSK 生图插件发布

此仓库由 IPZSK 维护。保留原包身份 `@dickpy/dsh-imagegen`，以便已有插件原位更新并保留历史；发布渠道固定为本仓库 GitHub Release，禁止向原作者 npm 包发布。

1. 更新 package.json 与 src/protocol.ts 中的版本。
2. 执行构建和测试，使用 npm pack --ignore-scripts 生成 tgz。
3. 创建相同版本的 GitHub Release 并上传 tgz（不要覆盖已发布附件）。
4. 在 IPZSK 开发者中心提交 Release URL，超级管理员审核上架。
5. 在客户端插件市场安装或更新；重启后生效。

插件使用主程序提供的 DSH Host/Client 接口，调用 IPZSK 后台的通用模型通道。主程序无需随插件重新打包。更新接口不兼容时，需要先发布兼容客户端。
