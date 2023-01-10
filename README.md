# suzume

<img src="./logo.png" width="700">

**SU**stainable **Z**ookeep & **U**pdate **ME**chanism

### 開発環境の構築

- [Nomadの公式のVagrantfile](https://raw.githubusercontent.com/hashicorp/nomad/master/demo/vagrant/Vagrantfile)からVMを構築します
- 参照: https://developer.hashicorp.com/nomad/tutorials/get-started/get-started-install#use-vagrant

```bash
# VagrantのBoxの起動
$ vagrant up

# VagrantのBoxにSSH接続
$ vagrant ssh

# Nomadの開発用のエージェント(Client/Server両用)の起動
$ sudo nomad agent -dev -bind=0.0.0.0

# Web UIを開く
$ open 192.168.56.10:4646

# サンプルのジョブ(Redis)の作成(HTTP API経由)
$ curl --request POST --data @example.json http://192.168.56.10:4646/v1/jobs

# VagrantのBoxの削除
$ vagrant destroy
```
