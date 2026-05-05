# 炮门演员争霸赛 - v1.2 备份

## 备份信息
- **版本**: v1.2
- **备份时间**: 2026-05-05
- **备份人**: 小牛 🐂

## 数据库导出
- **editions 表**: 5 条记录
- **rounds 表**: 40 条记录

## 版本特性（v1.2）
1. ✅ 届次倒序显示（最新一届排在最左边，默认选中）
2. ✅ 加演员弹窗改为多选（复选框列表，可同时勾选多个演员）
3. ✅ 已添加演员禁用（已在录入区的演员，复选框变灰禁用，标注"已添加"）
4. ✅ 录入区演员名可编辑（直接修改卡片上的名字，实时同步）
5. ✅ UTF-8 乱码修复
6. ✅ `renderLogs` 模板字符串 bug 修复
7. ✅ `result` 字段缺失修复

## 文件清单
- `Actor_Online.v1.2.html` - v1.2 版本完整 HTML 文件
- `Actor_Online.html` - 当前线上版本（与 v1.2 相同）
- `editions_v1.2.json` - 届次数据导出
- `rounds_v1.2.json` - 对局数据导出

## 恢复方法
1. 将 `Actor_Online.v1.2.html` 重命名为 `Actor_Online.html` 并部署
2. 在 Supabase SQL Editor 中执行：
   ```sql
   DELETE FROM rounds;
   DELETE FROM editions;
   ```
3. 使用 Supabase Dashboard 或 API 导入 `editions_v1.2.json` 和 `rounds_v1.2.json`

## 线上地址
https://leafknowsautumn.github.io/paomen-actor/Actor_Online.html

## GitHub 备份
- Tag: `v1.2`
- 备份目录: `backups/v1.2/`
- 仓库: https://github.com/LeafKnowsAutumn/paomen-actor
