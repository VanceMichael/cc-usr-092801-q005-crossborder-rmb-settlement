# 跨境人民币收付与风险额度协调

编排跨境人民币贸易依据、渠道指令、风险额度、回执和更正。

## 参与方与事实

主要参与方包括银行跨境业务团队、企业客户、合规复核人员、资金放行人员、境内外清算机构。领域资料记录以下已经确认的事实：

- 人民币跨境收付金额保持较大规模
- 多边数字货币桥交易增长
- 人民币清算网络连接多国机构

## 业务约束

- 贸易依据版本
- 金额守恒
- 渠道选择
- 额度占用
- 更正恢复

`contracts/context.schema.json` 描述资料结构，`fixtures/context.json` 提供不含真实身份信息的示例，`src/settlement_context.py` 负责读取和校验这些资料。

## 开发命令

运行测试：

```bash
python3 -m unittest discover -s tests -v
```

编译检查：

```bash
python3 -m compileall -q src
```

两条命令只读取仓库内文件，不需要连接外部业务系统。
