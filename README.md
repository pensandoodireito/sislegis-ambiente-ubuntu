# Ambiente Ubuntu para execução do SISLEGIS

Você pode utilizar este ambiente de várias formas:

1. Através do Ubuntu instalado em tua própria máquina;
2. Através do Vagrant (numa máquina com qualquer sistema operacional suportado por ele);
3. Através do Docker (melhor que usar o Vagrant se você estiver num Linux);

## Clonando e configurando este projeto

```
git clone http://github.com/pensandoodireito/sislegis-ambiente-ubuntu
cd sislegis-ambiente-ubuntu
cp config.exemplo config
vim config
```

## Montando o ambiente através do Vagrant

```bash
vagrant up
vagrant ssh
sudo apt-get -y update
sudo apt-get -y upgrade
/vagrant/instalar
logout
vagrant ssh
```

## Montando o ambiente numa instalação Ubuntu
