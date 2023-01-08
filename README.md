# suzume

<img src="./logo.png" width="700">

**SU**stainable **Z**ookeep & **U**pdate **ME**chanism

### 開発環境の構築

- [Nomadの公式のVagrantfile](https://raw.githubusercontent.com/hashicorp/nomad/master/demo/vagrant/Vagrantfile)からVMを構築します
- 参照: https://developer.hashicorp.com/nomad/tutorials/get-started/get-started-install#use-vagrant

```bash
$ vagrant up
$ vagrant ssh
$ sudo nomad agent -dev -bind=0.0.0.0
```
