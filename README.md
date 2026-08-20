<!--
# This is the name of the snap. The name that is registered on the snap store and also the name of the cli command.
snap-name: qwen3-8
# This name is just a friendly name for the snap, it can be used in the documentation
snap-friendly-name: Qwen 3.8
# URL to model card from the model publisher
model-card: https://huggingface.co/unsloth/Qwen3.8-27B-GGUF
# The port that the inference snap will use for its API server.
http-port: 8356
# The port that the inference snap will use for its webui server.
webui-http-port: 8357
# Optimizations
engines: cpu, nvidia-gpu
-->

# Qwen 3.8

[![qwen3-8](https://snapcraft.io/qwen3-8/badge.svg)](https://snapcraft.io/qwen3-8)

Qwen3.8 is the most capable generation in the Qwen open-model family to date.
Built on the architectural foundation of Qwen3.5, Qwen3.8 delivers substantial gains across coding, professional work, research, and long-horizon agentic tasks. Qwen3.8-27B brings these advances to a compact, deployment-friendly dense model: a native vision-language model that understands images and videos, with flexible thinking control, designed to carry complex, multi-step tasks through to completion with greater reliability.

Use this snap to quickly install an optimized environment for local inference with Qwen3.8.

The snap includes the following hardware-optimized inference engines:

* cpu: Optimized for x64 and ARM (armv8, armv9) CPUs
* nvidia-gpu: CUDA-enabled GPU acceleration

The most suitable engine is automatically selected based on the available hardware.

#### Install
```
sudo snap install qwen3-8
```

#### Run
```
qwen3-8
```

> [!TIP]
> Some accelerators require extra [drivers](https://documentation.ubuntu.com/inference-snaps/how-to/setup/drivers/) to be usable with this snap.

## Resources

📚 **[Documentation](https://documentation.ubuntu.com/inference-snaps/)**, learn how to use inference snaps

💬 **[Discussions](https://github.com/canonical/inference-snaps/discussions)**, ask questions and share ideas

🐛 **[Issues](https://github.com/canonical/inference-snaps/issues)**, report bugs and request features

## Build and install from source

Clone the repo:
```shell
git clone https://github.com/canonical/qwen3.8-snap
cd qwen3.8-snap
```

Initialize the development environment:
```shell
make init
```

Build and install snap:
```shell
make build
make install
```
