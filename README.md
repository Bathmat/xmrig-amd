# XMRig AMD

:warning: **[Monero will change PoW algorithm on October 18](https://github.com/xmrig/xmrig/issues/753), all miners and proxy should be updated to [v2.8+](https://github.com/xmrig/xmrig-amd/releases/tag/v2.8.0-rc)** :warning:

[![Github All Releases](https://img.shields.io/github/downloads/xmrig/xmrig-amd/total.svg)](https://github.com/MoneroOcean/xmrig-amd/releases)
[![GitHub release](https://img.shields.io/github/release/xmrig/xmrig-amd/all.svg)](https://github.com/MoneroOcean/xmrig-amd/releases)
[![GitHub Release Date](https://img.shields.io/github/release-date-pre/xmrig/xmrig-amd.svg)](https://github.com/MoneroOcean/xmrig-amd/releases)
[![GitHub license](https://img.shields.io/github/license/xmrig/xmrig-amd.svg)](https://github.com/MoneroOcean/xmrig-amd/blob/master/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/xmrig/xmrig-amd.svg)](https://github.com/MoneroOcean/xmrig-amd/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/xmrig/xmrig-amd.svg)](https://github.com/MoneroOcean/xmrig-amd/network)

XMRig is high performance Monero (XMR) OpenCL miner, with the official full Windows support.

GPU mining part based on [Wolf9466](https://github.com/OhGodAPet) and [psychocrypt](https://github.com/psychocrypt) code.

* This is the AMD (OpenCL) GPU mining version, there is also a [CPU version](https://github.com/MoneroOcean/xmrig) and [NVIDIA GPU version](https://github.com/MoneroOcean/xmrig-nvidia).
* [Roadmap](https://github.com/MoneroOcean/xmrig/issues/106) for next releases.

:warning: Suggested values for GPU auto configuration can be not optimal or not working, you may need tweak your threads options. Please fell free open an [issue](https://github.com/MoneroOcean/xmrig-amd/issues) if auto configuration suggest wrong values.

<img src="https://i.imgur.com/TFncsi7.png" width="696" >

#### Table of contents
* [Features](#features)
* [Download](#download)
* [Usage](#usage)
* [Build](https://github.com/MoneroOcean/xmrig-amd/wiki/Build)
* [Donations](#donations)
* [Release checksums](#release-checksums)
* [Contacts](#contacts)

## Features
* High performance.
* Official Windows support.
* Support for backup (failover) mining server.
* CryptoNight-Lite support for AEON.
* Automatic GPU configuration.
* Nicehash support.
* It's open source software.

## Download
* Binary releases: https://github.com/MoneroOcean/xmrig-amd/releases
* Git tree: https://github.com/MoneroOcean/xmrig-amd.git
  * Clone with `git clone https://github.com/MoneroOcean/xmrig-amd.git`  :hammer: [Build instructions](https://github.com/MoneroOcean/xmrig-amd/wiki/Build).

## Usage
Use [config.xmrig.com](https://config.xmrig.com/amd) to generate, edit or share configurations.

### Command line options
```
  -a, --algo=ALGO           cryptonight (default) or cryptonight-lite
  -o, --url=URL             URL of mining server
  -O, --userpass=U:P        username:password pair for mining server
  -u, --user=USERNAME       username for mining server
  -p, --pass=PASSWORD       password for mining server
  -k, --keepalive           send keepalived for prevent timeout (need pool support)
  -r, --retries=N           number of times to retry before switch to backup server (default: 5)
  -R, --retry-pause=N       time to pause between retries (default: 5)
      --opencl-devices=N    list of OpenCL devices to use.
      --opencl-launch=IxW   list of launch config, intensity and worksize
      --opencl-affinity=N   affine GPU threads to a CPU
      --opencl-platform=N   OpenCL platform index
      --no-color            disable colored output
      --donate-level=N      donate level, default 5% (5 minutes in 100 minutes)
      --user-agent          set custom user-agent string for pool
  -B, --background          run the miner in the background
  -c, --config=FILE         load a JSON-format configuration file
  -l, --log-file=FILE       log all output to a file
      --nicehash            enable nicehash support
      --print-time=N        print hashrate report every N seconds
      --api-port=N          port for the miner API
      --api-access-token=T  access token for API
      --api-worker-id=ID    custom worker-id for API
  -h, --help                display this help and exit
  -V, --version             output version information and exit
```

## Donations
Default donation 5% (5 minutes in 100 minutes) can be reduced to 1% via command line option `--donate-level`.

* XMR: `48edfHu7V9Z84YzzMa6fUueoELZ9ZRXq9VetWzYGzKt52XU5xvqgzYnDK9URnRoJMk1j8nLwEVsaSWJ4fhdUyZijBGUicoD`
* BTC: `1P7ujsXeX7GxQwHNnJsRMgAdNkFZmNVqJT`

## Release checksums
### SHA-256
```
c07fd13fbbae7f4a45928147defd3eef534ce25b84a6c47a2ff145e8c8b64d64 xmrig-amd-2.8.0-xenial-amd64.tar.gz/xmrig-amd-2.8.0/xmrig-amd
d713cec83e40de84bfef486dcca5900e2110f4f379e2980a90a4b6cea7ba6037 xmrig-amd-2.8.0-xenial-amd64.tar.gz/xmrig-amd-2.8.0/xmrig-amd-notls
59bd4261e2120302f9757412750f79bc92deb027d1ab53c1551b06fcd81d3505 xmrig-amd-2.8.0-win64.zip/xmrig-amd.exe
2b4f9974470ec50f7ed5ff06a9928ef9b24faa73c7dadd31e36984c98016e73c xmrig-amd-2.8.0-win64.zip/xmrig-amd-notls.exe
```

## Contacts
* support@xmrig.com
* [reddit](https://www.reddit.com/user/XMRig/)
* [twitter](https://twitter.com/xmrig_dev)
