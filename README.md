# NonceMiner

NonceMiner is a cross-platform mining client built with the [Electron](https://www.electronjs.org/) framework.  
Its underlying mining logic is powered by the open-source software [XMRig](https://github.com/xmrig/xmrig).  
With a simple graphical interface, you can easily participate in **Nonce token mining** on the GEB network and earn corresponding **Nonce tokens** as rewards.

---

## ✨ Features

1. 🧠 **CPU/GPU Friendly Mining**: Mine using your CPU or GPU to earn Nonce tokens based on your hash power on the GEB network.  
2. 🔄 **Token Exchange**: Instantly swap your Nonce tokens for the underlying mining tokens within the GEB network.  
3. 💸 **Instant Withdrawal**: Withdraw your mining tokens from the GEB network at any time.  
4. 🌐 **Multi-Coin Support**: Currently supports **XMR (Monero)** mining; more tokens will be supported in future versions.

---

## 📥 Installation & Usage

### Installation

1. Visit the [Releases page](../../releases)  
2. Download the appropriate installer or archive for your operating system:  
   - Windows: `.exe` installer  
   - macOS: `.dmg` / `.zip`  
   - Linux：`.tar.gz`
3. Run the installer or extract the archive, then launch the application to start mining.

⚠️ **Note for Windows Users**  
Since NonceMiner uses `xmrig` as the mining backend, some antivirus software may falsely flag it as a virus.  
You can add the installation folder to the exclusion list in **Windows Security → Virus & Threat Protection**, to prevent the system from blocking it.

### CLI Version (Linux)

Download and extract:
```
wget https://github.com/nonceworld/NonceMiner/releases/download/v0.2.0/nonceminer-linux-0.2.0.tar.gz
tar -zxvf nonceminer-0.2.0.tar.gz
cd nonceminer-0.2.0
./miner start --user {$evmAddress},{$wasmAddress}@{$worker}
```

evmAddress: Your EVM address

wasmAddress: Your GEB WASM address (optional)

worker: A name used to distinguish different machines you run the miner on

Example:
```
./miner start --user 0xdadB0d80178819F2319190D340ce9A924f783711,5Grux3pkj5adMKksEabeabMVHAsehvJ91s9WubQt7DvzqsSq@worker001
```

Other supported commands:
```
./miner status
./miner stop
./miner stop --miner=XMR
./miner stop --miner=XTMGPU
```

You may also edit the config.yaml file in the directory to add extra command arguments for the mining software.

---

## 📝 Disclaimer

NonceMiner is a mining client built on open-source software. Please comply with local laws and regulations when using it.
Users are solely responsible for any risks and resource consumption involved in the mining process.
