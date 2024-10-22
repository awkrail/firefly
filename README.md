# firefly
Yet another multimodal video feature extractor.

# Features
- unimodal: audio-only, visual-only
- multimodal: audio, visual, text
- multi GPU: multiple GPU supports
- multilingual: english, japanese VLM backbones
- synchronization: same-dimensional audio-visual feature (sequence length should be same)

# Libraries
FFmpeg
```
apt install ffmpeg
```

Pytorch
```
pip install torch==2.1.0 torchvision==0.16.0 torchaudio==2.1.0 torchtext==0.16.0 --index-url https://download.pytorch.org/whl/cu118
```

# Models
### Vision-only
- [x] : TIMM models

Action
- [ ] : I3D
- [ ] : Slowfast
- [ ] : VideoMAE

Optical flow
- [ ] : RAFT

Audio-only
- [ ] : PANNs
- [ ] : VGGish

Image-text
- [x] : CLIP
- [x] : Japanese CLIP

Video-text
- [ ] : CLIP4Clip
- [ ] : InternVideo

Audio-text
- [x] : CLAP (Microsoft)
- [ ] : CLAP (LAION)

# Test
```
pytest tests
```

# Mypy + Ruff
```
mypy firefly
ruff check firefly
```