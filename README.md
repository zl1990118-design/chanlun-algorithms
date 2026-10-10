# 缠论算法库

> 缠中说禅技术分析的开源实现集合。收录各开源项目（保留原 LICENSE 与版本），供行情分析、选股、量化研究引用。

## 收录清单

| 子库 | 来源 | 语言 | 说明 | 许可 |
|---|---|---|---|---|
| [czsc](https://github.com/zl1990118-design/czsc) | [waditu/czsc](https://github.com/waditu/czsc) | Rust | 缠论算法工程化标杆：分型/笔/中枢 + 220+ 信号函数，形式化验证首选 | MIT |
| [chan.py](https://github.com/zl1990118-design/chan.py) | [Vespa314/chan.py](https://github.com/Vespa314/chan.py) | Python | 开放式缠论框架：形态学/动力学买卖点、多级别K线联立、区间套策略、可视化 | MIT |
| [chanlun-pro](https://github.com/zl1990118-design/chanlun-pro) | [yijixiuxin/chanlun-pro](https://github.com/yijixiuxin/chanlun-pro) | Python | 缠论量化工具：笔/段/中枢/买卖点，多市场数据接入；**注意：核心引擎 src/chanlun/core 为加密专有组件，需授权运行** | Apache-2.0（core 除外） |

## 快速上手

各子库为完整独立工程，直接进入对应目录查看 README 运行。

## 常用算法入口

- **包含处理 / 分型 / 笔**：`czsc/crates/czsc-core/src/analyze/{mod.rs,utils.rs}`；`chan.py/chanpy/fx.py`；`chanlun-pro/chanlun/`
- **中枢**：`czsc/crates/czsc-core/src/objects/zs.rs`
- **买卖点**：`czsc/crates/czsc-signals/src/`（byi 等）；`chan.py/chanpy/bs.py`
- **多级别联立 / 区间套**：`chan.py/chanpy/analyze.py`

## 维护

- 各子库保留上游历史与许可声明，更新时拉取上游最新版。
- 新增收录建议先确认许可兼容。
