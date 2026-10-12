# Wan Animate and Crazyrouter video API guide

Updated 2026-10-12. Wan is the Alibaba/Wan team's model family. It is distinct from ByteDance's Seedance.

## What Wan Animate does

[Wan2.2-Animate-14B](https://github.com/Wan-Video/Wan2.2#run-wan-animate) takes a reference character image and a driving video. It supports character animation and replacement. Follow the upstream repository for weights, preprocessing, inference and license terms.

This is different from a general text-to-video model. Do not send `wan-2.2` to `/v1/chat/completions` to generate a video. The previous examples and unsupported per-video price claims have been removed.

## Using hosted video APIs

Check [Crazyrouter's Wan documentation](https://docs.crazyrouter.com/en/video/wan) and [current catalogue](https://crazyrouter.com/en/models) for the exact hosted model and operation. Upstream availability of Wan Animate does not imply that the same operation is hosted by this gateway.

Video APIs use task submission and status/result retrieval. The model determines the route, required images/video, duration, size, audio settings and billing unit. Use the documented task API rather than Chat Completions. A submitted task ID is not a finished video.

For price and commercial-use decisions, consult the [current pricing](https://crazyrouter.com/en/pricing) and the applicable model/provider license. No blanket quality, speed, free-tier or commercial-use guarantee is made here.
