# Lower-cost Flovart API examples

[Local-language guide](README_zh-CN.md) · [Upstream](https://github.com/avabbbb/Flovart) · [Attribution](UPSTREAM.md)

Experimental opt-in UserScript JSON provider proposal; preserve RunningHub release path and shared durable Workflow authority. Real independent API outputs tested; Browser Workflow, durable Artifact import and creative-host acceptance remain unverified.

## Examples

![Original image](assets/gpt-image-2-vip-399025ccb7.png)

# Model prices and case charges

2026-10-23 · USD · international site (.com). Sorted by case amount; image quotes remain explicitly pending.

| Model | Conditions | Model price | This case |
|---|---|---:|---:|
| gpt-image-2(VIP) | low / 1K / 1 image | $0.0019/image quoted | Actual settlement pending |
| seedance-2-5 | 480p / first frame / audio off | ≈ $0.096040/s in this sample | $0.388 settled / 4.04s |

Video $/s is the actual settled amount divided by decoded duration; it is an observed average, not a fixed tariff.

Token-rate reference at this Key’s request time: $10/1M total tokens. Different prompts, references, duration, resolution and pricing changes may alter cost.

![Video preview](assets/seedance-2-5-5fd3aa62a5.jpg)

[Play actual MP4](assets/seedance-2-5-5fd3aa62a5.mp4)

Original first-frame input: [PNG](assets/first-frame.png). Requested 4s, decoded 4.04s; 480p, 16:9, audio off. Actual charge $0.388.

## Reuse

Set `TOAPIS_API_KEY` privately on the server. Python 3.10+, standard library for API calls.

```sh
python unified_client.py --model gpt-image-2-vip --prompt-file prompts/image.txt --max-usd .05
# Review price before authorizing one paid request:
python unified_client.py --model gpt-image-2-vip --prompt-file prompts/image.txt --max-usd .05 --live --run-id reviewed-image-01
```

```sh
python unified_client.py --model seedance-2-5 --prompt-file prompts/video.txt --image assets/first-frame.png --max-usd .50
# Add --live --run-id reviewed-video-01 only after price review.
```

The same stable run identity resumes its saved task. Retain `.state` privately. An uncertain submission is not resubmitted automatically. Seedance Global models are disabled.

## Provider contribution

[Candidate integration and acceptance boundaries](integration/README.md). Real API calls, recorded protocol/byte boundaries and native application acceptance are distinct checks. Existing providers, sponsor/referral links and local workflows are preserved. No trial credits have been issued and no official endorsement is implied.

[Register at ToAPIs](https://toapis.com/login?aff=BEWR)
