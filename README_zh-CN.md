# 更低成本的 Flovart

[English](README.md) · [Upstream](https://github.com/avabbbb/Flovart)

图片显示本次 Key 查询报价，实际结算待确认；视频显示已确认实扣。本页是独立 API 案例与接入提案，完整产品内流程待共同验收。

## 案例与费用

![Case](assets/gpt-image-2-vip-399025ccb7.png)

gpt-image-2(VIP): **$0.0019/image** (quoted).

![Video](assets/seedance-2-5-5fd3aa62a5.jpg)

[MP4](assets/seedance-2-5-5fd3aa62a5.mp4) · seedance-2-5 · **$0.388/request**, ≈ **$0.096040/s**, 4.04s / 480p.

在服务端私有环境配置 TOAPIS_API_KEY。先不加 --live 查询价格，审核后再显式提交。保留相同 --run-id 以续查已有任务，不自动重提不确定的付费 POST。

```sh
python unified_client.py --model gpt-image-2-vip --prompt-file prompts/image.txt --max-usd .05
```

[Full parameters, scripts and limits](README.md#reuse) · [Provider candidate](integration/README.md) · [Prices](PRICING.md)

[ToAPIs](https://toapis.com/login?aff=BEWR)
