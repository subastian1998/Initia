# dayak
{
  "$schema": "../../chain.schema.json",
  "chain_name": "initia",
  "chain_id": "initiation-1",
  "website": "https://initia.xyz",
  "pretty_name": "Initia",
  "status": "live",
  "network_type": "testnet",
  "bech32_prefix": "init",
  "daemon_name": "initiad",
  "node_home": "$HOME/.initia",
  "key_algos": ["secp256k1"],
  "slip44": 118,
  "fees": {
    "fee_tokens": [
      {
        "denom": "uinit",
        "fixed_min_gas_price": 0.15,
        "low_gas_price": 0.15,
        "average_gas_price": 0.15,
        "high_gas_price": 0.4
      },
      {
        "denom": "ueth"
      },
      {
        "denom": "uusdc"
      },
      {
        "denom": "utia"
      }
    ]
  },
  "staking": {
    "staking_tokens": [
      {
        "denom": "uinit"
      },
      {
        "denom": "move/dbf06c48af3984ec6d9ae8a9aa7dbb0bb1e784aa9b8c4a5681af660cf8558d7d"
      },
      {
        "denom": "move/a2b0d3c8e53e379ede31f3a361ff02716d50ec53c6b65b8c48a81d5b06548200"
      },
      {
        "denom": "move/b134ae6786f10ef74294e627d2519b63b7c742a6735f98682929fea9a84744d2"
      }
    ]
  },
  "codebase": {
    "git_repo": "https://github.com/initia-labs/initia",
    "recommended_version": "v0.2.8",
    "compatible_versions": ["v0.2.8"],
    "binaries": {
      "linux/amd64": "https://initia.s3.ap-southeast-1.amazonaws.com/initiation-1/initia_v0.2.8_Linux_x86_64.tar.gz",
      "linux/arm64": "https://initia.s3.ap-southeast-1.amazonaws.com/initiation-1/initia_v0.2.8_Linux_aarch64.tar.gz",
      "darwin/amd64": "https://initia.s3.ap-southeast-1.amazonaws.com/initiation-1/initia_v0.2.8_Darwin_x86_64.tar.gz",
      "darwin/arm64": "https://initia.s3.ap-southeast-1.amazonaws.com/initiation-1/initia_v0.2.8_Darwin_aarch64.tar.gz"
    },
    "genesis": {
      "genesis_url": "https://initia.s3.ap-southeast-1.amazonaws.com/initiation-1/genesis.json"
    },
    "versions": []
  },
  "description": "Initia Testnet",
  "peers": {
    "seeds": [],
    "persistent_peers": []
  },
  "apis": {
    "rpc": [
      {
        "address": "https://rpc.initiation-1.initia.xyz",
        "provider": "Foundation"
      }
    ],
    "rest": [
      {
        "address": "https://lcd.initiation-1.initia.xyz",
        "provider": "Foundation"
      }
    ],
    "api": [
      {
        "address": "https://api.initiation-1.initia.xyz",
        "provider": "Foundation"
      }
    ],
    "grpc": [
      {
        "address": "grpc://35.247.153.122:9090",
        "provider": "Foundation"
      }
    ]
  },
  "explorers": [
    {
      "kind": "initia scan",
      "url": "https://scan.testnet.initia.xyz/initiation-1",
      "tx_page": "https://scan.testnet.initia.xyz/initiation-1/txs/${txHash}",
      "account_page": "https://scan.testnet.initia.xyz/initiation-1/accounts/${accountAddress}"
    }
  ],
  "faucets": [
    {
      "kind": "faucet",
      "url": "https://faucet.testnet.initia.xyz/"
    }
  ],
  "images": [
    {
      "png": "https://raw.githubusercontent.com/initia-labs/initia-registry/main/testnets/initia/images/INIT.png",
      "svg": "https://raw.githubusercontent.com/initia-labs/initia-registry/main/testnets/initia/images/INIT.svg"
    }
  ],
  "logo_URIs": {
    "png": "https://raw.githubusercontent.com/initia-labs/initia-registry/main/testnets/initia/images/INIT.png",
    "svg": "https://raw.githubusercontent.com/initia-labs/initia-registry/main/testnets/initia/images/INIT.svg"
  },
  "metadata": {
    "is_l1": true,
    "ibc_channels": [
      {
        "chain_id": "minimove-1",
        "port_id": "transfer",
        "channel_id": "channel-0",
        "version": "ics20-1"
      },
      {
        "chain_id": "minimove-1",
        "port_id": "nft-transfer",
        "channel_id": "channel-1",
        "version": "ics721-1"
      },
      {
        "chain_id": "miniwasm-1",
        "port_id": "transfer",
        "channel_id": "channel-4",
        "version": "ics20-1"
      },
      {
        "chain_id": "miniwasm-1",
        "port_id": "nft-transfer",
        "channel_id": "channel-5",
        "version": "ics721-1"
      }
    ],
    "assetlist": "https://raw.githubusercontent.com/initia-labs/initia-registry/main/testnets/initia/assetlist.json"
  }
}
