


## Dependencies

- Python 3.9
- torchvision == 0.12.0
- numpy
- timm == 0.4.12
- einops
- yacs

## Train Models from Scratch

- **To train `S2E-Swin-T/S/B` on ImageNet from scratch, run:**

```shell
python -m torch.distributed.launch --nproc_per_node=8 main.py --cfg ./cfgs/S2E_swin_t.yaml --data-path <imagenet-path> --output <output-path>


python -m torch.distributed.launch --nproc_per_node=8 main.py --cfg ./cfgs/S2E_swin_s.yaml --data-path <imagenet-path> --output <output-path>

python -m torch.distributed.launch --nproc_per_node=8 main.py --cfg ./cfgs/S2E_swin_b.yaml --data-path <imagenet-path> --output <output-path>
