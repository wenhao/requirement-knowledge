---
type: domain-index
product_line: 商城
module: 订单
title: 订单域首页
owner: 李四
review_status: confirmed
knowledge_status: active
disclosure_level: L1
current_baseline: v2.3
updated: 2026-11-04
---

# 订单域首页

## 1. 域定位

订单域负责订单创建、支付结果处理、履约、取消、退款、状态流转，以及与会员、营销、库存、财务之间的关联。

## 2. 页面索引

| 类型 | 页面 | 状态 | 一句话说明 |
|---|---|---|---|
| 术语 | [待履约](术语-待履约.md) | confirmed / active | 已支付但尚未完成履约 |
| 术语 | [退款单](术语-退款单.md) | confirmed / active | 承载退款状态与金额的单据 |
| 规则 | [退款超时](规则-退款超时.md) | confirmed / active | 48 小时未发货自动全额退款 |
| 规则 | [取消订单](规则-取消订单.md) | confirmed / active | 未发货前可取消，发货后转售后 |
| 规则 | [重复退款拦截](规则-重复退款拦截.md) | confirmed / active | 同一退款意图只能成功一次 |
| 流程 | [下单到退款](流程-下单到退款.md) | confirmed / active | 从下单到退款完成的状态流转 |
| 需求 | [虚拟商品退款例外](需求-虚拟商品退款例外.md) | confirmed / active | 虚拟商品不适用自动退款规则 |
| 场景 | [预售订单退款](场景-预售订单退款.md) | confirmed / active | 预售定金与尾款退款场景 |
| 风险 | [重复退款](风险-重复退款.md) | confirmed / active | 并发回调可能导致重复退款 |
| 常见问题 | [预售退款](常见问题-预售退款.md) | confirmed / active | 预售退款时效与尾款处理 |

## 3. 推荐阅读路径

### 编写退款需求

1. [订单域上下文包](_domain-context.md)
2. [退款超时](规则-退款超时.md)
3. [取消订单](规则-取消订单.md)
4. [虚拟商品退款例外](需求-虚拟商品退款例外.md)
5. [重复退款风险](风险-重复退款.md)

### 排查状态问题

1. [待履约](术语-待履约.md)
2. [下单到退款](流程-下单到退款.md)
3. [跨域退款与积分口径](../跨域/决策-退款与积分回退口径.md)
