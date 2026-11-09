# 输入输出契约

## 输入字段

| 键 | 名称 | 类型 | 必填 |
|---|---|---|---|
| `turnover_records` | 离职记录 | array | 是 |
| `staffing_data` | 编制与在岗数据 | array | 是 |
| `workload_data` | 工作量数据 | array | 否 |
| `performance_distribution` | 绩效分布 | array | 否 |
| `employee_survey` | 员工调查摘要 | array | 否 |
| `key_events` | 关键管理事件 | array | 否 |
| `campus_job_labels` | 校区与岗位标签 | array | 是 |
| `review_period` | 复盘周期 | string | 是 |

## 状态

- `completed`：核心成果完整，关键结论人工确认要求满足。
- `completed_with_limits`：至少一项实质成果，说明限制、已完成和受阻范围。
- `needs_input`：必填字段缺失。
- `needs_confirmation`：资料冲突或人工确认未完成。
- `failed`：计算或工具失败。

## 输出

- `组织健康诊断`：结构化条目数组，不允许空壳或占位文本。
- `离职风险热区`：结构化条目数组，不允许空壳或占位文本。
- `证据与反证`：结构化条目数组，不允许空壳或占位文本。
- `访谈提纲`：结构化条目数组，不允许空壳或占位文本。
- `改进计划`：结构化条目数组，不允许空壳或占位文本。
- `复测指标`：结构化条目数组，不允许空壳或占位文本。

完整机器契约见`contract/input.schema.json`、`contract/output.schema.json`和`contract/runtime_contract.json`。
