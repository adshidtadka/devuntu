# proect-k 開発環境用 vagrant VM

## Installation

### virtualbox

### vagrant

```sh
vagrant plugin install vagrant-vbguest

# いろいろインストールするので30分くらいかかる。ネット回線のいいところで実行する必要あり。
vagrant up

# VM 再起動
vagrant reload
```

失敗したっぽくても、 `...ignoring` とついていれば問題ないので無視して大丈夫です。

```
fatal: [192.168.33.10]: FAILED! => {"changed": true, "cmd": ["test", "-x", "/home/vagrant/.pyenv/bin/pyenv"], "delta": "0:00:00.005286", "end": "2017-10-20 08:55:42.714028", "failed": true, "msg": "non-zero return code", "rc": 1, "start": "2017-10-20 08:55:42.708742", "stderr": "", "stderr_lines": [], "stdout": "", "stdout_lines": []}
...ignoring
```

## Usage

### 普段

```sh
vagrant up
```

### 更新時

```sh
vagrant reload
vagrant provision
```



