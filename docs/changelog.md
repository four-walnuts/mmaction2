## Changelog

### v0.7.0 (30/9/2020)

**Highlights**

**New Features**
- Support to run real-time action recognition from web camera ([#171](https://github.com/open-mmlab/mmaction2/pull/171))
- Support to export the pytorch models to onnx ones. ([#160](https://github.com/open-mmlab/mmaction2/pull/160))
- Support to report mAP for ActivityNet with [CUHK17_activitynet_pred](http://activity-net.org/challenges/2017/evaluation.html). ([#176](https://github.com/open-mmlab/mmaction2/pull/176))

**ModelZoo**
- Add finetuning setting for SlowOnly. ([#173](https://github.com/open-mmlab/mmaction2/pull/173))

**Improvements**
- Support to run a demo with a video url ([#165](https://github.com/open-mmlab/mmaction2/pull/165))
- Add tutorial for adding a new learning rate updater ([#181](https://github.com/open-mmlab/mmaction2/pull/181))
- Add config name in meta info ([#183](https://github.com/open-mmlab/mmaction2/pull/183))
- Remove git hash in `__version__` ([#189](https://github.com/open-mmlab/mmaction2/pull/189))
- Check mmcv version ([#189](https://github.com/open-mmlab/mmaction2/pull/189))

**Bug Fixes**
- Fix the bug when using OpenCV to extract only RGB frames with original shape ([#184](https://github.com/open-mmlab/mmaction2/pull/187))
- Fix the bug of sthv2 `num_classes` from 339 to 174 ([#174](https://github.com/open-mmlab/mmaction2/pull/174), [#207](https://github.com/open-mmlab/mmaction2/pull/207))


### v0.6.0 (2/9/2020)

**Highlights**
- Support TIN, CSN, SSN, NonLocal
- Support FP16 training

**New Features**
- Support NonLocal module and provide ckpt in TSM and I3D ([#41](https://github.com/open-mmlab/mmaction2/pull/41))
- Support SSN ([#33](https://github.com/open-mmlab/mmaction2/pull/33), [#37](https://github.com/open-mmlab/mmaction2/pull/37), [#52](https://github.com/open-mmlab/mmaction2/pull/52), [#55](https://github.com/open-mmlab/mmaction2/pull/55))
- Support CSN ([#87](https://github.com/open-mmlab/mmaction2/pull/87))
- Support TIN ([#53](https://github.com/open-mmlab/mmaction2/pull/53))
- Support HMDB51 dataset preparation ([#60](https://github.com/open-mmlab/mmaction2/pull/60))
- Support encoding videos from frames ([#84](https://github.com/open-mmlab/mmaction2/pull/84))
- Support FP16 training ([#25](https://github.com/open-mmlab/mmaction2/pull/25))
- Enhance demo by supporting rawframe inference ([#59](https://github.com/open-mmlab/mmaction2/pull/59)), output video/gif ([#72](https://github.com/open-mmlab/mmaction2/pull/72))

**ModelZoo**
- Update Slowfast modelzoo ([#51](https://github.com/open-mmlab/mmaction2/pull/51))
- Update TSN, TSM video checkpoints ([#50](https://github.com/open-mmlab/mmaction2/pull/50))
- Add data benchmark for TSN ([#57](https://github.com/open-mmlab/mmaction2/pull/57))
- Add data benchmark for SlowOnly ([#77](https://github.com/open-mmlab/mmaction2/pull/77))
- Add BSN/BMN performance results with feature extracted by our codebase ([#99](https://github.com/open-mmlab/mmaction2/pull/99))

**Improvements**
- Polish data preparation codes ([#70](https://github.com/open-mmlab/mmaction2/pull/70))
- Improve data preparation scripts ([#58](https://github.com/open-mmlab/mmaction2/pull/58))
- Improve unittest coverage and minor fix ([#62](https://github.com/open-mmlab/mmaction2/pull/62))
- Support PyTorch 1.6 in CI ([#117](https://github.com/open-mmlab/mmaction2/pull/117))
- Support `with_offset` for rawframe dataset ([#48](https://github.com/open-mmlab/mmaction2/pull/48))
- Support json annotation files ([#119](https://github.com/open-mmlab/mmaction2/pull/119))
- Support `multi-class` in TSMHead ([#104](https://github.com/open-mmlab/mmaction2/pull/104))
- Support using `val_step()` to validate data for each `val` workflow ([#123](https://github.com/open-mmlab/mmaction2/pull/123))
- Use `xxInit()` method to get `total_frames` and make `total_frames` a required key ([#90](https://github.com/open-mmlab/mmaction2/pull/90))
- Add paper introduction in model readme ([#140](https://github.com/open-mmlab/mmaction2/pull/140))
- Adjust the directory structure of `tools/` and rename some scripts files ([#142](https://github.com/open-mmlab/mmaction2/pull/142))

**Bug Fixes**
- Fix configs for localization test ([#67](https://github.com/open-mmlab/mmaction2/pull/67))
- Fix configs of SlowOnly by fixing lr to 8 gpus ([#136](https://github.com/open-mmlab/mmaction2/pull/136))
- Fix the bug in analyze_log ([#54](https://github.com/open-mmlab/mmaction2/pull/54))
- Fix the bug of generating HMDB51 class index file ([#69](https://github.com/open-mmlab/mmaction2/pull/69))
- Fix the bug of using `load_checkpoint()` in ResNet ([#93](https://github.com/open-mmlab/mmaction2/pull/93))
- Fix the bug of `--work-dir` when using slurm training script ([#110](https://github.com/open-mmlab/mmaction2/pull/110))
- Correct the sthv1/sthv2 rawframes filelist generate command ([#71](https://github.com/open-mmlab/mmaction2/pull/71))
- `CosineAnnealing` typo ([#47](https://github.com/open-mmlab/mmaction2/pull/47))


### v0.5.0 (9/7/2020)

**Highlights**
- MMAction2 is released

**New Features**
- Support various datasets: UCF101, Kinetics-400, Something-Something V1&V2, Moments in Time,
  Multi-Moments in Time, THUMOS14
- Support various action recognition methods: TSN, TSM, R(2+1)D, I3D, SlowOnly, SlowFast, Non-local
- Support various action localization methods: BSN, BMN
- Colab demo for action recognition
