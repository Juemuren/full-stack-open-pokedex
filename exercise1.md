# Exercise 11.1

## Question 1

CI 设置中的一些常见步骤包括代码检查、测试和构建。在你选择的编程语言生态系统中，处理这些步骤的具体工具有哪些？

我选择的是 Go 编程语言

### 代码检查工具
- **静态检查**: `golangci-lint`、`staticcheck`、`revive`
- **安全扫描**: `gosec`、`govulncheck`
- **格式化**: `gofmt`、`goimports`

### 测试工具
- **单元测试**: `go test` + `testing`
- **基准测试**: `go test -bench`
- **模糊测试**: `go test -fuzz`

### 构建工具
- **跨平台编译**: `go build` + 设置 `GOOS` 和 `GOARCH` 环境变量
- **依赖管理**: `go mod`

## Question 2

除了 Jenkins 和 GitHub Actions 之外，还有哪些设置 CI 的替代方案？

### 云托管方案
- **GitLab CI/CD**: 与 GitLab 深度集成
- **CircleCI**: 配置简单，性能优秀
- **Travis CI**: 老牌选择，YAML 配置
- **Azure Pipelines**: 微软生态集成
- **Bitbucket Pipelines**: Bitbucket 原生集成
- **AWS CodePipeline**: AWS服务集成

### 自托管方案
- **Drone CI**: Go 语言开发，轻量级
- **Tekton**: Kubernetes 原生 CI/CD
- **Concourse**: 声明式管道配置

## Question 3

CI 设置是在自托管环境还是云环境中更好？为什么？你需要哪些信息来做这个决定？

### 自托管优势
- **数据控制**: 代码和流水线数据完全自控
- **定制灵活**: 完全自定义硬件和软件环境
- **成本可控**: 长期使用可能更经济
- **网络隔离**: 内网部署，访问速度快

### 云环境优势
- **维护简单**: 无需基础设施管理
- **弹性扩展**: 按需使用资源
- **开箱即用**: 快速启动，预集成了很多服务
- **全球分发**: 多区域部署能力

### 决策需要的信息

1. **安全要求**
   - 代码敏感性级别
   - 合规性要求
   - 数据驻留要求

2. **技术考量**
   - 现有基础设施
   - 团队技术能力
   - 集成需求

3. **经济因素**
   - 预算限制
   - 团队规模和使用频率
   - 长期成本预测

4. **业务需求**
   - 上市时间压力
   - 可扩展性需求
   - 可靠性要求
