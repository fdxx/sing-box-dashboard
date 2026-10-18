# sing-box dashboard

Web dashboard for sing-box.

## 与原版的区别

本分支基于 [SagerNet/sing-box-dashboard](https://github.com/SagerNet/sing-box-dashboard)，增加了以下交互改进：

- **出站组状态记忆**：`/groups` 页面会在本地分别保存各出站组的展开或收起状态，刷新页面或重新进入后自动恢复。没有保存记录时沿用后端返回的状态。
- **暂停/继续刷新连接**：`/connections` 页面右上角的三个点菜单左侧新增暂停按钮。暂停后，列表和详情固定显示暂停时的数据，仍可搜索、筛选和查看详情；后台继续接收数据，点击继续后显示最新数据。每次重新进入页面时默认继续刷新。
- **完整出站链**：连接列表右侧显示完整的路由链，包括经过的 selector、urltest 等出站组，顺序和 ` / ` 分隔方式与连接详情中的“链”一致。没有链信息时显示出站名称，较长的链会自动换行。

下方 Public instance 为原版的公共实例，不包含本分支的改动。

## Public instance

http://sing-box-dashboard.sagernet.org

For Chrome, you can use HTTPS, but not for other browsers.

Shortcut: dash.sing-box.app

## LICENSE

```
Copyright (C) 2022 by nekohasekai <contact-sagernet@sekai.icu>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.

In addition, no derivative work may use the name or imply association
with this application without prior consent.
```