# 组织健康与离职风险诊断示例

## 典型场景

某校区教师半年流失率升高，但薪酬与同城接近，需检查排班和管理关系。

## 具体示例

Agent 先提出负荷、管理、成长等竞争性假设，并设计访谈验证，不直接断言离职原因。

## 脱敏输入示例

```json
{
  "contract_version": "1.2.0",
  "data_status": "confirmed",
  "contains_sensitive_data": false,
  "requested_output_language": "zh-CN",
  "turnover_records": [
    {}
  ],
  "staffing_data": [
    {}
  ],
  "workload_data": [
    {}
  ],
  "performance_distribution": [
    {}
  ],
  "employee_survey": [
    {}
  ],
  "key_events": [
    {}
  ],
  "campus_job_labels": [
    {}
  ],
  "review_period": "复盘周期已核对（脱敏示例）",
  "resume_mode": "new"
}
```

## 预期处理

1. 运行输入契约校验。
2. 逐项核对输入来源、版本和口径。
3. 按`references/PROFESSIONAL_PLAYBOOK.md`完成专业分析。
4. 输出组织健康诊断、离职风险热区、改进计划等核心成果。
5. 由业务负责人确认输入事实、关键假设和最终成果适用范围后才可作为正式业务结论。

## 不应出现的输出

- 虚构政策、价格、人员、课程或客户事实。
- 以“暂无”“待完善”等占位文本冒充完成。
- 无依据的确定性判断或伪造人工签批。
