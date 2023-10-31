## Cleo : Cryptographic leakage evaluation of Hardware


The RISC-V instruction set architecture is known for its open-source and customizable design. One of the notable features of RISC-V is its modular and extensible nature, allowing developers to add custom instructions and extensions tailored to specific applications. One such security extension is the RISC-V Cryptography Extension (RISC-V Crypto). This extension enhances RISC-V processors with hardware acceleration for cryptographic operations, making it well-suited for secure computing tasks. In order to comply with standard architecture guidelines, RISC-V Crypto has developed proto-type hardware implementations in hardware description languages (e.g. Verilog).

 The device's power consumption fluctuates as it executes computations, responding to changing logic states and data processing. These current variations generate distinct patterns that enable the analysis of the ongoing operations. By observing these power consumption fluctuations and correlating them with specific computations, an adversary can deduce sensitive data, such as cryptographic keys or plaintext, without needing direct access to the internal memory or processes of the target device.


In this project, I propose a TVLA framework for RISC-V cryptography extension standardization work. This work will result in a complete power side-channel evaluation framework parallel to the existing test-based functional validation suite~\cite{rvcrypto_github} and functional formal verification suite~\cite{rvcrypto_github}. 

### Project Structure

Here is the folder structure. both [riscv-crypto](https://github.com/riscv/riscv-crypto/) and [xcrypto](https://github.com/scarv/xcrypto) are initialized as submodules.

```shell
├── dockerfile
│   └── dockerfile
├── eut # extenstions under test
│   ├── riscv-crypto
│   └── xcrypto
└── readme.md
```

Use following commands to initiate submodules

```shell
git submodule update --init --recursive
```

### Environement

```shell

docker pull ....
docker run ........
docker exec ........

```
