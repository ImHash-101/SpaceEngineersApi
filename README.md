space engineers ingame script API
=
太空工程师 API · 内置 · 程序块
-
***
太空工程师目前使用的库为 .net.4.6.1

编译语言为 C#

如果你想在太空工程师中编写脚本或者设计大型MOD，本API可以一定程度的帮助到你。

制作mod的同学，请直接翻阅目录

转载请注明出处，谢谢。

## 快速链接
* [游戏内脚本API](#游戏内脚本API)
* [游戏的接口API](#游戏的接口API)
* [游戏内Vage函数](#游戏内Vage函数)

<a name="游戏内脚本API"></a>
## 游戏内脚本API
***
脚本目录API链接

|[**方块父类**](#方块父类)|[**VRage.Game**](./SE-2/VRage.Game/VRage/Game/ModAPI/Ingame)|
|-----|-----|
|[**特殊方块**](#特殊方块)|[**SpaceEngineers.Game**](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame)|
|[**基础方块**](#基础方块)|[**Sandbox.Common**](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame)|

<a name="方块父类"></a>
### 方块父类

|类名|类型|注备|功能|
|----|----|----|----|
|[IMyCubeBlock](./SE-2/VRage.Game/VRage/Game/ModAPI/Ingame/IMyCubeBlock.cs)|方块|子类|获取方块信息|
|[IMyCubeGrid](./SE-2/VRage.Game/VRage/Game/ModAPI/Ingame/IMyCubeGrid.cs)|网格|子类|获取网格信息|
|[IMyEntity](./SE-2/VRage.Game/VRage/Game/ModAPI/Ingame/IMyEntity.cs)|实例|父类|获取实例信息|
|[IMyInventory](./SE-2/VRage.Game/VRage/Game/ModAPI/Ingame/IMyInventory.cs)|仓库||获取仓库信息|
|[IMyInventoryItem](./SE-2/VRage.Game/VRage/Game/ModAPI/Ingame/IMyInventoryItem.cs)|物品||获取物品信息|
|[IMyInventoryOwner](./SE-2/VRage.Game/VRage/Game/ModAPI/Ingame/IMyInventoryOwner.cs)|背包|废弃|获取背包信息|
|[IMySlimBlock](./SE-2/VRage.Game/VRage/Game/ModAPI/Ingame/IMySlimBlock.cs)|方块|特殊|获取方块特殊信息|
|[MyInventoryItemExtension](./SE-2/VRage.Game/VRage/Game/ModAPI/Ingame/MyInventoryItemExtension.cs)|物品扩展|方法|设定自定义ID？|


### 方块脚本API
<a name="基础方块"></a>
基础方块

|类名|类型|注备|功能|
|----|----|----|----|
|[DoorStatus](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/DoorStatus.cs)|状态枚举|门|门的状态|
|[FlightMode](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/FlightMode.cs)|状态枚举|远程模块|无人飞行模式|
|[IMyAdvancedDoor](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyAdvancedDoor.cs)|高级门类|暂时无效|特定获取|
|[IMyAirtightDoorBase](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyAirtightDoorBase.cs)|密封门类|特定|特定获取-密闭门|
|[IMyAirtightHangarDoor](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyAirtightDoorBase.cs)|气密门|特定|特定获取-密闭门-气密门|
|[IMyAirtightSlideDoor](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyAirtightHangarDoor.cs)|滑动门|特定|特定获取-密闭门-滑动门|
|[IMyAssembler](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyAssembler.cs)|装配机|面板|装配机面板读写|
|[IMyAttachableTopBlock](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyAttachableTopBlock.cs)|顶部连接方块|属性获取|连接状态|
|[IMyBatteryBlock](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyBatteryBlock.cs)|电池|面板|电池面板读写|
|[IMyBeacon](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyBeacon.cs)|信标|范围|信标范围设置|
|[IMyBlockGroup](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyBlockGroup.cs)|方块编组|方法|程序块语句、获取类|
|[IMyCameraBlock](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyCameraBlock.cs)|摄像头|方法/面板|摄像头特殊功能读写|
|[IMyCargoContainer](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyCargoContainer.cs)|货仓|特定|特定获取-货仓|
|[IMyCockpit](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyCockpit.cs)|驾驶舱|状态|驾驶舱状态获取|
|[IMyCollector](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyCollector.cs)|收集器|面板|特定获取-收集器|
|[IMyConveyor](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyConveyor.cs)|输送机|特定|特定获取-输送机|
|[IMyConveyorSorter](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyConveyorSorter.cs)|分拣机|面板|分拣机设置|
|[IMyConveyorTube](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyConveyorTube.cs)|输送管|特定|特定获取-输送管|
|[IMyCryoChamber](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyCryoChamber.cs)|低温箱/冷冻室/休眠仓|特定|特定获取-休眠仓|
|[IMyDecoy](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyDecoy.cs)|诱饵|特定|特定获取-诱饵|
|[IMyDoor](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyDoor.cs)|门|父类|门面板设置|
|[IMyExtendedPistonBase](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyExtendedPistonBase.cs)|活塞|活塞头|特定获取-活塞头|
|[IMyFunctionalBlock](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyFunctionalBlock.cs)|功能方块|父类|属性读写|
|[IMyGasGenerator](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyGasGenerator.cs)|气体制造机|面板|气体制造机设置|
|[IMyGasTank](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyGasTank.cs)|气罐|面板|气罐面板读取|
|[IMyGridProgramRuntimeInfo](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyGridProgramRuntimeInfo.cs)|程序块运行信息|网格/程序块|程序块运行相关|
|[IMyGridTerminalSystem](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyGridTerminalSystem.cs)|终端信息|网格/程序块|程序块调用相关|
|[IMyGyro](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyGyro.cs)|陀螺仪|面板|陀螺仪设置|
|[IMyJumpDrive](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyJumpDrive.cs)|跃迁引擎|面板|跃迁设置|
|[IMyLargeTurretBase](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyLargeTurretBase.cs)|自动炮塔|面板|属性设置|
|[IMyLaserAntenna](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyLaserAntenna.cs)|激光天线|面板|属性设置|
|[IMyLightingBlock](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyLightingBlock.cs)|灯|面板|灯设置|
|[IMyMechanicalConnectionBlock](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyMechanicalConnectionBlock.cs)|机械连接方块|属性获取|连接状态|
|[IMyMotorAdvancedRotor](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyMotorAdvancedRotor.cs)|高级转子|特定|特定获取|
|[IMyMotorAdvancedStator](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyMotorAdvancedStator.cs)|高级转子座|特定|特定获取|
|[IMyMotorBase](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyMotorBase.cs)|转子座|特定|特定获取|
|[IMyMotorRotor](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyMotorRotor.cs)|转子|特定|特定获取|
|[IMyMotorStator](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyMotorStator.cs)|转子|面板|基础设定|
|[IMyMotorSuspension](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyMotorSuspension.cs)|转子|隐藏面板|特殊设定|
|[IMyOreDetector](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyOreDetector.cs)|矿物探测器|面板|范围设定|
|[IMyOxygenGenerator](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyOxygenGenerator.cs)|氧气制造机|被替代|氧气制造机设置|
|[IMyOxygenTank](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyOxygenTank.cs)|氧气罐|被替代|面板设置|
|[IMyPassage](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyPassage.cs)|过道|特定|特定获取|
|[IMyPistonBase](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyPistonBase.cs)|活塞|面板|面板设置|
|[IMyPistonTop](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyPistonTop.cs)|活塞头|特定|特定获取|
|[IMyProductionBlock](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyProductionBlock.cs)|生产方块|父类|生产设置|
|[IMyProgrammableBlock](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyProgrammableBlock.cs)|程序方块|面板|面板设置|
|[IMyProjector](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyProjector.cs)|投影仪|面板|面板设置|
|[IMyRadioAntenna](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyRadioAntenna.cs)|天线|面板|面板设定|
|[IMyReactor](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyReactor.cs)|反应堆|面板|面板设定|
|[IMyRefinery](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyRefinery.cs)|精炼厂|特定|特定获取|
|[IMyReflectorLight](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyReflectorLight.cs)|射灯|特定|特定获取|
|[IMyRemoteControl](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyRemoteControl.cs)|远程控制|面板|面板设置|
|[IMySensorBlock](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMySensorBlock.cs)|探测器|面板|探测器功能读写|
|[IMyShipConnector](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyShipConnector.cs)|飞船连接器|面板|连接设置|
|[IMyShipController](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyShipController.cs)|飞船控制|网格|飞船特殊属性读写|
|[IMyShipDrill](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyShipDrill.cs)|钻头|面板|面板|
|[IMyShipGrinder](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyShipGrinder.cs)|切割机|特定|特定获取|
|[IMyShipToolBase](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyShipToolBase.cs)|飞船基础工具|面板|面板|
|[IMyShipWelder](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyShipWelder.cs)|焊机|面板|面板|
|[IMySmallGatlingGun](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMySmallGatlingGun.cs)|小型加特林|面板|面板|
|[IMySmallMissileLauncher](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMySmallMissileLauncher.cs)|小型导弹|面板|面板|
|[IMySmallMissileLauncherReload](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMySmallMissileLauncherReload.cs)|可装填导弹发射器|特定|特定获取|
|[IMyTerminalBlock](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyTerminalBlock.cs)|终端父类|面板|大部分方块的面板功能|
|[IMyTextPanel](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyTextPanel.cs)|文字面板LCD|面板|面板设置|
|[IMyThrust](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyThrust.cs)|推进器|面板|推进器设置|
|[IMyUpgradableBlock](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyUpgradableBlock.cs)|升级方块|属性|获取|
|[IMyUpgradeModule](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyUpgradeModule.cs)|升级模组|属性|获取|
|[IMyUserControllableGun](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyUserControllableGun.cs)|武器控制|状态|状态获取|
|[IMyWarhead](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyWarhead.cs)|弹头|面板|面板设置|
|[IMyWheel](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/IMyWheel.cs)|车轮|特定|特定获取|
|[MyAssemblerMode](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/MyAssemblerMode.cs)|装配机状态|枚举|状态|
|[MyConveyorSorterMode](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/MyConveyorSorterMode.cs)|输送机模式|枚举|状态|
|[MyDetectedEntityInfo](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/MyDetectedEntityInfo.cs)|探测器实体信息|类|属性|
|[MyDetectedEntityType](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/MyDetectedEntityType.cs)|探测器实体类型|枚举|属性|
|[MyGridProgram](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/MyGridProgram.cs)|程序块语句|特定|程序相关|
|[MyInventoryItemFilter](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/MyInventoryItemFilter.cs)|储存过滤|类|属性|
|[MyJumpDriveStatus](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/MyJumpDriveStatus.cs)|跃迁引擎状态|枚举|状态|
|[MyLaserAntennaStatus](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/MyLaserAntennaStatus.cs)|激光天线状态|枚举|状态|
|[MyPlanetElevation](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/MyPlanetElevation.cs)|高度属性|枚举|属性|
|[MyProductionItem](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/MyProductionItem.cs)|生产列表|类|属性|
|[MyShipConnectorStatus](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/MyShipConnectorStatus.cs)|连接状态|枚举|属性|
|[MyShipMass](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/MyShipMass.cs)|质量|类|属性|
|[MyShipVelocities](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/MyShipVelocities.cs)|速度|类|属性|
|[MyTransmitTarget](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/MyTransmitTarget.cs)|信号|枚举|定义|
|[MyWaypointInfo](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/MyWaypointInfo.cs)|路径|类|属性|
|[PistonStatus](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/PistonStatus.cs)|远程坐标|枚举|定点动作|
|[TerminalActionParameter](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/TerminalActionParameter.cs)|终端|类|功能|
|[TerminalBlockExtentions](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/TerminalBlockExtentions.cs)|终端|类|功能扩展|
|[UpdateFrequency](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/UpdateFrequency.cs)|更新频率|枚举|定义|
|[UpdateType](./SE-2/Sandbox.Common/Sandbox/ModAPI/Ingame/UpdateType.cs)|更新类型|枚举|定义|

<a name="特殊方块"></a>
特殊方块

|类名|类型|注备|功能|
|----|----|----|----|
|[IMyAirVent](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyAirVent.cs)|排风扇|面板|设置|
|[IMyArtificialMassBlock](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyArtificialMassBlock.cs)|人工质量|特定|特定获取|
|[IMyButtonPanel](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyButtonPanel.cs)|按钮面板|面板|设置|
|[IMyControlPanel](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyControlPanel.cs)|终端|特定|特定获取|
|[IMyGravityGeneratorBase](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyGravityGeneratorBase.cs)|重力发生器基类|面板|设置|
|[IMyGravityGenerator](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyGravityGenerator.cs)|重力发生器|面板|设置|
|[IMyGravityGeneratorSphere](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyGravityGeneratorSphere.cs)|球型重力发生器|面板|设置|
|[IMyInteriorLight](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyInteriorLight.cs)|室内灯|特定|特定获取|
|[IMyLandingGear](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyLandingGear.cs)|着陆器/起落架|面板|设置|
|[IMyLargeConveyorTurretBase](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyLargeConveyorTurretBase.cs)|炮塔传输系统|面板|设置|
|[IMyLargeGatlingTurret](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyLargeGatlingTurret.cs)|加特林炮台|特定|特定获取|
|[IMyLargeInteriorTurret](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyLargeInteriorTurret.cs)|室内机枪|特定|特定获取|
|[IMyLargeMissileTurret](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyLargeMissileTurret.cs)|飞弹炮台|特定|特定获取|
|[IMyMedicalRoom](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyMedicalRoom.cs)|医疗仓|特定|特定获取|
|[IMyOxygenFarm](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyOxygenFarm.cs)|氧气农场|面板|设置|
|[IMyParachute](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyParachute.cs)|降落伞|面板|设置|
|[IMyShipMergeBlock](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyShipMergeBlock.cs)|合并块|面板|设置|
|[IMySolarPanel](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMySolarPanel.cs)|太阳能板|面板|获取|
|[IMySoundBlock](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMySoundBlock.cs)|音效方块|面板|设置|
|[IMySpaceBall](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMySpaceBall.cs)|空间球|面板|设置|
|[IMyTimerBlock](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyTimerBlock.cs)|计时器|面板|设置|
|[IMyVirtualMass](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/IMyVirtualMass.cs)|虚拟质量|面板|获取|
|[VentStatus](./SE-2/SpaceEngineers.Game/SpaceEngineers/Game/ModAPI/Ingame/VentStatus.cs)|气密|枚举|状态|

<a name="游戏的接口API"></a>
## 游戏的接口API
***

目录位置

|[**普通接口**](#普通接口)|[**Sandbox.Common**](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces)|
|-----|-----|
|     |[**VRage.Game**](./SE-2/VRage.Game/VRage/Game/ModAPI/Interfaces)|
|[**终端接口**](#终端接口)|[**Sandbox.Common-Terminal**](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal)|

<a name="普通接口"></a>
普通接口

|类名|类型|注备|功能|
|----|----|----|----|
|[ITerminalAction](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/ITerminalAction.cs)|终端动作接口|面板+属性|获取|
|[ITerminalProperty＜TValue＞](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/ITerminalProperty!1.cs)|终端属性接口|面板|读写|
|[ITerminalProperty](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/ITerminalProperty.cs)|终端属性接口|ID|获取|
|[TerminalPropertyExtensions](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/TerminalPropertyExtensions.cs)|终端属性扩展接口|ID|读写|
|[IMyCameraController](./SE-2/VRage.Game/VRage/Game/ModAPI/Interfaces/IMyCameraController.cs)|||||
|[IMyControllableEntity](./SE-2/VRage.Game/VRage/Game/ModAPI/Interfaces/IMyControllableEntity.cs)|||||
|[IMyDecalHandler](./SE-2/VRage.Game/VRage/Game/ModAPI/Interfaces/IMyDecalHandler.cs)|||||
|[IMyDecalProxy](./SE-2/VRage.Game/VRage/Game/ModAPI/Interfaces/IMyDecalProxy.cs)|||||
|[IMyDestroyableObject](./SE-2/VRage.Game/VRage/Game/ModAPI/Interfaces/IMyDestroyableObject.cs)|||||
|[MoveInformation](./SE-2/VRage.Game/VRage/Game/ModAPI/Interfaces/MoveInformation.cs)|||||

<a name="终端接口"></a>
Terminal](终端接口)

|类名|类型|注备|功能|
|----|----|----|----|
|[IMyTerminalAction](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal/IMyTerminalAction.cs)|终端动作接口|面板|读写|
|[IMyTerminalControlButton](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal/IMyTerminalControlButton.cs)|||||
|[IMyTerminalControlCheckbox](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal/IMyTerminalControlCheckbox.cs)|||||
|[IMyTerminalControlColor](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal/IMyTerminalControlColor.cs)||||||
|[IMyTerminalControlCombobox](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal/IMyTerminalControlCombobox.cs)|||||
|[IMyTerminalControl](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal/IMyTerminalControl.cs)|||||
|[IMyTerminalControlLabel](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal/IMyTerminalControlLabel.cs)|||||
|[IMyTerminalControlListbox](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal/IMyTerminalControlListbox.cs)|||||
|[IMyTerminalControlOnOffSwitch](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal/IMyTerminalControlOnOffSwitch.cs)|||||
|[IMyTerminalControlProperty＜TValue＞](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal/IMyTerminalControlProperty!1.cs)|||||
|[IMyTerminalControlSeparator](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal/IMyTerminalControlSeparator.cs)|||||
|[IMyTerminalControlSlider](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal/IMyTerminalControlSlider.cs)|||||
|[IMyTerminalControlTextbox](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal/IMyTerminalControlTextbox.cs)|||||
|[IMyTerminalControlTitleTooltip](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal/IMyTerminalControlTitleTooltip.cs)|||||
|[IMyTerminalValueControl＜TValue＞](./SE-2/Sandbox.Common/Sandbox/ModAPI/Interfaces/Terminal/IMyTerminalValueControl!1.cs)|||||


<a name="游戏内Vage函数"></a>
## 游戏内Vage函数
***

[**游戏内Vage函数**](./SE-2/VRage.Math/VRageMath)

|    |    |    |
|----|----|----|
|[Base27Directions](./SE-2/VRage.Math/VRageMath/Base27Directions.cs)|[Line](./SE-2/VRage.Math/VRageMath/Line.cs)|[Quaternion](./SE-2/VRage.Math/VRageMath/Quaternion.cs)|
|[Base6Directions](./SE-2/VRage.Math/VRageMath/Base6Directions.cs)|[LineD](./SE-2/VRage.Math/VRageMath/LineD.cs)|[QuaternionD](./SE-2/VRage.Math/VRageMath/QuaternionD.cs)|
|[BoundingBox2](./SE-2/VRage.Math/VRageMath/BoundingBox2.cs)|[MathHelper](./SE-2/VRage.Math/VRageMath/MathHelper.cs)|[Ray](./SE-2/VRage.Math/VRageMath/Ray.cs)|
|[BoundingBox2D](./SE-2/VRage.Math/VRageMath/BoundingBox2D.cs)|[MathHelperD](./SE-2/VRage.Math/VRageMath/MathHelperD.cs)|[RayD](./SE-2/VRage.Math/VRageMath/RayD.cs)|
|[BoundingBox2I](./SE-2/VRage.Math/VRageMath/BoundingBox2I.cs)|[Matrix](./SE-2/VRage.Math/VRageMath/Matrix.cs)|[Rectangle](./SE-2/VRage.Math/VRageMath/Rectangle.cs)|
|[BoundingBox](./SE-2/VRage.Math/VRageMath/BoundingBox.cs)|[MatrixD](./SE-2/VRage.Math/VRageMath/MatrixD.cs)|[RectangleF](./SE-2/VRage.Math/VRageMath/RectangleF.cs)|
|[BoundingBoxD](./SE-2/VRage.Math/VRageMath/BoundingBoxD.cs)|[MatrixI](./SE-2/VRage.Math/VRageMath/MatrixI.cs)|[SerializableRange](./SE-2/VRage.Math/VRageMath/SerializableRange.cs)|
|[BoundingBoxExtensions](./SE-2/VRage.Math/VRageMath/BoundingBoxExtensions.cs)|[MyBlockOrientation](./SE-2/VRage.Math/VRageMath/MyBlockOrientation.cs)|[Spatial](./SE-2/VRage.Math/VRageMath/Spatial)|
|[BoundingBoxI](./SE-2/VRage.Math/VRageMath/BoundingBoxI.cs)|[MyBounds](./SE-2/VRage.Math/VRageMath/MyBounds.cs)|[SymetricSerializableRange](./SE-2/VRage.Math/VRageMath/SymetricSerializableRange.cs)|
|[BoundingFrustum](./SE-2/VRage.Math/VRageMath/BoundingFrustum.cs)|[MyCuboid](./SE-2/VRage.Math/VRageMath/MyCuboid.cs)|[SymmetricSerializableRange](./SE-2/VRage.Math/VRageMath/SymmetricSerializableRange.cs)|
|[BoundingFrustumD](./SE-2/VRage.Math/VRageMath/BoundingFrustumD.cs)|[MyCuboidSide](./SE-2/VRage.Math/VRageMath/MyCuboidSide.cs)|[TreeUserAction＜Ｔ＞](./SE-2/VRage.Math/VRageMath/TreeUserAction!1.cs)|
|[BoundingFrustumExtensions](./SE-2/VRage.Math/VRageMath/BoundingFrustumExtensions.cs)|[MyDynamicAABBTree](./SE-2/VRage.Math/VRageMath/MyDynamicAABBTree.cs)|[Vector2B](./SE-2/VRage.Math/VRageMath/Vector2B.cs)|
|[BoundingSphere](./SE-2/VRage.Math/VRageMath/BoundingSphere.cs)|[MyDynamicAABBTreeD](./SE-2/VRage.Math/VRageMath/MyDynamicAABBTreeD.cs)|[Vector2](./SE-2/VRage.Math/VRageMath/Vector2.cs)|
|[BoundingSphereD](./SE-2/VRage.Math/VRageMath/BoundingSphereD.cs)|[MyLineSegmentOverlapResult＜Ｔ＞](./SE-2/VRage.Math/VRageMath/MyLineSegmentOverlapResult!1.cs)|[Vector2D](./SE-2/VRage.Math/VRageMath/Vector2D.cs)|
|[BoxCornerEnumerator](./SE-2/VRage.Math/VRageMath/BoxCornerEnumerator.cs)|[MyMath](./SE-2/VRage.Math/VRageMath/MyMath.cs)|[Vector2I](./SE-2/VRage.Math/VRageMath/Vector2I.cs)|
|[Capsule](./SE-2/VRage.Math/VRageMath/Capsule.cs)|[MyMortonCode3D](./SE-2/VRage.Math/VRageMath/MyMortonCode3D.cs)|[Vector3B](./SE-2/VRage.Math/VRageMath/Vector3B.cs)|
|[CapsuleD](./SE-2/VRage.Math/VRageMath/CapsuleD.cs)|[MyOrientedBoundingBox](./SE-2/VRage.Math/VRageMath/MyOrientedBoundingBox.cs)|[Vector3](./SE-2/VRage.Math/VRageMath/Vector3.cs)|
|[Color](./SE-2/VRage.Math/VRageMath/Color.cs)|[MyOrientedBoundingBoxD](./SE-2/VRage.Math/VRageMath/MyOrientedBoundingBoxD.cs)|[Vector3D](./SE-2/VRage.Math/VRageMath/Vector3D.cs)|
|[ColorExtensions](./SE-2/VRage.Math/VRageMath/ColorExtensions.cs)|[MyQuad](./SE-2/VRage.Math/VRageMath/MyQuad.cs)|[Vector3Extensions](./SE-2/VRage.Math/VRageMath/Vector3Extensions.cs)|
|[CompressedPositionOrientation](./SE-2/VRage.Math/VRageMath/CompressedPositionOrientation.cs)|[MyQuadD](./SE-2/VRage.Math/VRageMath/MyQuadD.cs)|[Vector3I](./SE-2/VRage.Math/VRageMath/Vector3I.cs)|
|[ContainmentType](./SE-2/VRage.Math/VRageMath/ContainmentType.cs)|[MyShort4](./SE-2/VRage.Math/VRageMath/MyShort4.cs)|[Vector3INormalEqualityComparer](./SE-2/VRage.Math/VRageMath/Vector3INormalEqualityComparer.cs)|
|[CubeFace](./SE-2/VRage.Math/VRageMath/CubeFace.cs)|[MyTransform](./SE-2/VRage.Math/VRageMath/MyTransform.cs)|[Vector3I_RangeIterator](./SE-2/VRage.Math/VRageMath/Vector3I_RangeIterator.cs)|
|[CurveContinuity](./SE-2/VRage.Math/VRageMath/CurveContinuity.cs)|[MyTransformD](./SE-2/VRage.Math/VRageMath/MyTransformD.cs)|[Vector3S](./SE-2/VRage.Math/VRageMath/Vector3S.cs)|
|[Curve](./SE-2/VRage.Math/VRageMath/Curve.cs)|[MyUShort4](./SE-2/VRage.Math/VRageMath/MyUShort4.cs)|[Vector3UByte](./SE-2/VRage.Math/VRageMath/Vector3UByte.cs)|
|[CurveKeyCollection](./SE-2/VRage.Math/VRageMath/CurveKeyCollection.cs)|[NullableVector3DExtensions](./SE-2/VRage.Math/VRageMath/NullableVector3DExtensions.cs)|[Vector3Ushort](./SE-2/VRage.Math/VRageMath/Vector3Ushort.cs)|
|[CurveKey](./SE-2/VRage.Math/VRageMath/CurveKey.cs)|[NullableVector3Extensions](./SE-2/VRage.Math/VRageMath/NullableVector3Extensions.cs)|[Vector4](./SE-2/VRage.Math/VRageMath/Vector4.cs)|
|[CurveLoopType](./SE-2/VRage.Math/VRageMath/CurveLoopType.cs)|[PackedVector](./SE-2/VRage.Math/VRageMath/PackedVector)|[Vector4D](./SE-2/VRage.Math/VRageMath/Vector4D.cs)|
|[CurveTangent](./SE-2/VRage.Math/VRageMath/CurveTangent.cs)|[Plane](./SE-2/VRage.Math/VRageMath/Plane.cs)|[Vector4I](./SE-2/VRage.Math/VRageMath/Vector4I.cs)|
|[Gjk](./SE-2/VRage.Math/VRageMath/Gjk.cs)|[PlaneD](./SE-2/VRage.Math/VRageMath/PlaneD.cs)|[Vector4UByte](./SE-2/VRage.Math/VRageMath/Vector4UByte.cs)|
|[GjkD](./SE-2/VRage.Math/VRageMath/GjkD.cs)|[PlaneIntersectionType](./SE-2/VRage.Math/VRageMath/PlaneIntersectionType.cs)|
|[HyperSphereHelpers](./SE-2/VRage.Math/VRageMath/HyperSphereHelpers.cs)|[Point](./SE-2/VRage.Math/VRageMath/Point.cs)|

