# MultiplayerSession: UE5.7 编译兼容修正（无联机检验）

## 状态
- version：5.7
- 已通过编译
- 无联机检验

## 修改内容
- 在`MultiplayerSessionSubsystem.cpp`中，将已移除的`SEARCH_PRESENCE`搜索键迁移为`SEARCH_LOBBIES`
- 添加`Online/OnlineSessionName.h`使得`SEARCH_LOBBIES`声名可见
- 在`WBP_Menu`的class defaults中配置`Is Focusable`,代替运行时赋值