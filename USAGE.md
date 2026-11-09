# 使用说明

## 适用任务

某校区教师半年流失率升高，但薪酬与同城接近，需检查排班和管理关系。

## 准备输入

脱敏离职数据、编制/工时、绩效分布、培训、员工调查、关键事件、校区/岗位标签。使用前先脱敏姓名、联系方式和与任务无关的敏感信息。

## 操作步骤

1. 确定范围
2. 数据脱敏
3. 趋势与分层
4. 生成根因假设
5. 设计访谈/验证
6. 制定改进项目
7. 复测

## 校验命令

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 状态使用

- `completed`：核心成果完整。
- `completed_with_limits`：只完成可验证部分，并说明受阻范围。
- `needs_input`：缺少关键输入。
- `needs_confirmation`：资料冲突或需人工确认。
- `failed`：工具或计算失败，提供恢复动作。

## 人工确认

业务负责人复核输入事实、关键假设和最终成果适用范围后，成果才可进入正式业务使用。
