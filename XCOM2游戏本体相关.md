# 游玩建议
## 购买安装建议
* 由于存在需要装扮 DLC 才能成立的 Mod 框架（Alien Hunters Community Highlander），故需要购买全部 DLC 并安装。
* 需要下载 [Alternate Mod Launcher - AML启动器](https://github.com/X2CommunityCore/xcom2-launcher/wiki/Installation)，不要将其放在游戏目录中
* 盗版及启动器要放在纯英文路径，不要放在 C 盘已有文件夹下

## 启动及创建战役建议
* 启动前将微软输入法改为其他输入法或美式键盘，多数 BUG 与此相关
* 将根目录下 XCom2-WarOfTheChosen\Engine\Config\BaseEngine.ini 中找到 set AllowJoystickInput，等号后面改成 0，预防地球界面无限左移问题
* 以管理员模式启动 AML，通过 AML 进入游戏，启动 WOTC 而非原版，WOTC 包含全部原版内容
* 初次启动游戏有几率黑屏卡死闪退，此时需要根据显卡搜索强制游戏以窗口化启动的方案，或进入游戏时按 Alt+Enter 切窗口
* 分辨率设置最好为 16:9 或 16:10，其它分辨率最好使用窗口模式
* 不要开启平滑帧率，与大多数信息显示类 Mod 冲突
* 开新战役不要开教程，剧情任务勿用自定义人物进行交互
* 输入名字时记得关闭手柄连接
* 战术传承包少用模组，使用铜人模组进行铁人挑战
* 每 10 小时连续游戏时间需重启电脑一次；应对优化问题和崩溃卡顿，多关机降温、重启电脑
* 崩溃日志位置：我的文档\my games\XCOM2 War of the Chosen\XComGame\Logs

## 游玩流程/BUG 相关建议
* 游戏内人物/目标卡到地图外或掉出地面消失，需重启任务
* 使用 Mod 技能/动作时崩溃，需加载上一个存档或排查并禁用模组
* Bad Image 错误，需重新下载[Visual C++ Redistributable Packages for Visual Studio 2013](https://www.microsoft.com/zh-CN/download/details.aspx?id=40784)
* 过场动画和任务简报无声音，需切换英文后重启游戏再切换为简中
* XCom2.exe - 无法找到入口/XCom2.exe - Entry Point Not Found/Message The map specified on the commandline……'LauncherPatcher.exe' could not be found. Would you like to load the default map instead? 三个错误都是因杀毒软件误杀
* Error detected attempting load of package 尝试加载程序包时检测到错误，重新下载 package 后跟的内容，比如 TLE1Sword_SF.upk 对应战术传承包 DLC，需要 Steam-DLC 取消勾选该包再勾选
* 研究弹药时选择弹药研究立刻完成的反抗军命令导致弹药研究无限暂停，取消该命令
* LOGO 动画后黑屏，ESC 无法返回，退出到桌面卡死，
  1. Steam 禁用云存档
  2. 删除 我的文档\my games\XCOM2 War of the Chosen 文件夹和游戏根目录下 \XCom2-WarOfTheChosen\Engine\Config 文件夹
  3. Steam 验证游戏完整性
  4. 进入游戏后按 Alt+Enter 切换窗口模式
* 显示正在运行游戏但打不开游戏，重启电脑，无效则尝试使用手机热点进入
* 攻击刺客天选者基地，刺客一直不现身也无法攻击石棺
  + 至少保留一颗伤害性榴弹，没有就重置任务
  + 控制台输入 dropunit chosenassassin 1 1 刷出天选者
  + 石棺没血条则切换到带榴弹的队员，控制台输入 toggleunlimitedammo 和 Giveactionpoints 99
  + 将伤害榴弹丢到石板中间 5 次左右出血条，出血条后再丢一次可继续任务
* 头颅接入器导致画面卡住，盲按空格或回车，切键鼠进行游戏
* 最后一关不能用带中继器的死神打第一个化身，触发中继器会卡关


## AML 启动器与 Mod 相关
* 在 AML 设置的启动命令参数和快速切换命令参数栏中添加参数（需加前面的减号，需用空格隔开）
  + -review 禁用开发模式
  + -allowConsole 启用控制台，需配合 -language=int 切换语言为英文使用
  + -noStartUpMovies 无LOGO画面
  + -noRedScreens 禁用红屏
* 启动前备份 AML 根目录中的  steam_api64.dll，并将游戏目录中的同名文件复制粘贴（覆盖）至 AML 根目录
* 若初次启动时错误地选择游戏导致报错，则进入启动器根目录，将 steam_appid.txt 中的 268500 换为 882100 或反过来
* “无法检测 Steam！”则重启 Steam
* 模组显示“-1字节”，右键取消订阅-订阅，重启 AML
* 若只在使用 Mod 后出现问题，勾选 AML 右上角 regenerateinis 重生模式以测试单 AML 时的游戏稳定性
* Error detected attempting load of package 弹窗需确定 package 来自什么模组/游戏文件并重下/替换内容
* 不自动下载模组，尝试点掉 Steam 离线模式，验证游戏完整性，订阅一个其它的模组后取消订阅

## Mod 崩溃处理办法


# Mod 选择建议
## 总览
* 多用 Mod 修改非设置项而非修改原文件
* 备份并清理 我的文档\My Games\XCOM2 War of the Chosen\XComGame\Config 文件夹+重启两次游戏可解决 Mod 本身造成的崩溃问题
* Steam 验证游戏完整性可解决被 Mod 修改的游戏文件所引发的问题
* 进入游戏字体显示为口口，则需要将汉化文件编码改成 ANSI

## 防坏档模组
* Bronzeman Mode 铜人模式，用于替换铁人模式预防坏档，仅允许在基地保存
* Mission Launch Auto Save 开始任务前自动保存（防御复仇者任务除外）
* Remove Missing Mods 一次性 Mod，随装随用用完删除，在SL界面生成一个按钮用于自动移除存档中的已弃用 Mod 内容，若成功，主菜单应为暗影舱+死神的背景，此后应重启游戏，与 Rename And Reorganize Campaign 冲突

## 易崩溃模组
* Free Camera Rotation 自由摄像机视角，易出现白屏卡死
* Quick Soldier Info 快速士兵信息，易导致防御复仇者号任务卡住不动，临时禁用可解决
* Tactical Options 战术选项，可能导致存档时闪退

## 易冲突模组
* Long War of the Chosen 对游戏整体的大改，有白名单
* RPG Overhaul 角色养成相关大改，有白名单
* Improved Weapon Upgrade UI 与 Grimy's Loot Mod 冲突，将后者换成 TeslaRage's Loot Mod 即可
* Peek From Concealment UI Fix 与 Gotcha Again 冲突，将后者的 XComEngine.ini 中的 +ModClassOverrides=(BaseGameClass="XComPathingPawn",ModClass="XComPathingPawn_GA") 删除

## 稳定性模组
* Additional Soldier Console Commands 士兵控制台指令
  1. LevelUpSelectedSoldier 改变士兵等级，从 0 开始
  2. RebuildSelectedSoldiersClass 改变士兵职业/技能/属性
  3. RebuildAllSoldiersClass 刷新所有士兵的技能树和随机技能，修复技能树图标缺失和 Missing 'LocFriendlyName' for None 等 BUG
  4. SetSelectedSoldiersStat 改变选定士兵的属性
  5. SetSelectedSoldiersComInt 改变选定士兵的智商
  6. ReloadWeapon 选定士兵重新装弹

## QOL 模组
* Shot Hud Ability Position Exchanger 始终保持一些动作在固定位置，防止多技能模组挤占
* [WOTC] Unlimited Ability Icons 无限动作图标
* Fixed Sniper Hotkeys 修复狙击手热键与 Evac All 的不兼容

## 部分模组说明
* Better Tactical Zoom Out 调整摄像机缩放高度，默认 T 放大，G 缩小，按住鼠标中键缩为最小，删除会坏档

# 汉化相关
1. 汉化需要用到语言原文件，可以复制文件后改后缀名，xx.int Mod文本英文，xx.chn 中文，xx.cht 繁中
2. 汉化时需要注意不要修改尖括号文本，其为动态提取的文本内容，常与数值有关。
'''no
英文：
LocHelpText="Send the Gremlin to resupply a target ally, granting them +1 Action Point. <Ability:ACTIONPROTOCOLRS_CHARGES/> Charges per Mission."
中文：
LocHelpText="发送小精灵至目标并提供额外一点行动力. 消耗 <Ability:ACTIONPROTOCOLRS_CHARGES/> 行动点"
'''
3. 支持无限撤回/备份/版本管理的文本编辑器
4. 文本检索软件/插件
5. 文本比对软件/插件


# 参考材料
* [暗之小白-XCOM2 Mod 中文爱好者-知乎](https://www.zhihu.com/people/shen-jing-wa-42-28/posts)
  + [Mod 推荐](https://zhuanlan.zhihu.com/p/568841471)
* [超简单汉化-3DM](https://bbs.3dmgame.com/thread-5653078-1-1.html)
* [控制台指令](https://steamcommunity.com/sharedfiles/filedetails/?id=2608547705)
