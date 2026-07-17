# FeeFlow Miniapp

FeeFlow 是企业费控移动端，基于 uni-app + Vue 3 + TypeScript，支持员工提交报销、上传发票、审批费用、登记付款和查看预算余额。

## 关联仓库

- [FeeFlow Admin + Go Gin API](https://github.com/xrlnewman/feeflow-admin)
- [个人博客项目页](https://field-notes-2fi.pages.dev/projects/feeflow-platform/)

```bash
npm install
npm test
npm run dev:h5
```

配置 `VITE_API_BASE_URL` 或 `UNI_APP_API_BASE_URL` 后调用后台 `/api/v1`；写操作自动携带 `Idempotency-Key`，网络错误会回退虚构演示数据。状态依次经过费用申请 → 发票 → 预算校验 → 审批 → 付款确认。

MIT © xrlnewman
