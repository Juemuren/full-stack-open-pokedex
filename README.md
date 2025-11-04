# Full Stack Open Part11

## 一些说明

- [11.10-11.12](https://fullstackopen.com/en/part11/deployment#exercises-11-10-11-12-fly-io) 由于没有信用卡，部署相关的练习无法完成。后续 CI 中的部署步骤仅用简单打印信息来模拟。
- [11.19] 该练习决定不完成。因为首先得测试 `workflows` 本身是正确的，然后再测试配置的 `schedule` 是正确的。后者等待事件触发又需要很长时间。而确认 `schedule` 没问题后又要把它撤销掉，以免浪费服务器资源。我已经有了一个配置了 `schedule` 的[仓库](https://github.com/Juemuren/ScoopBucket)，因此这个练习我就不完成了。
- [11.20-11.21] 我的一个[博客](https://github.com/Juemuren/DevNotes)已经使用了 `Github Actions`，且暂时不想更改该仓库的分支保护措施。故这两个练习跳过。