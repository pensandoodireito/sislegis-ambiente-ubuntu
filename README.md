# Ambiente Ubuntu para execução do SISLEGIS

Você pode utilizar este ambiente de várias formas:

1. Através do Ubuntu instalado em tua própria máquina;
2. Através do Vagrant (numa máquina com qualquer sistema operacional suportado por ele);

## Clonando e configurando este projeto

```bash
git clone http://github.com/pensandoodireito/sislegis-ambiente-ubuntu
cd sislegis-ambiente-ubuntu
cp config.exemplo config
vim config
source config
```

No Linux:
```bash
echo "f=\"$PWD/config\"; [ -f \"\$f\" ] && source \"\$f\"; unset f" >> ~/.bashrc
```

No OSX:
```bash
echo "f=\"$PWD/config\"; [ -f \"\$f\" ] && source \"\$f\"; unset f" >> ~/.profile
```

## Montando o ambiente através do Vagrant

```bash
vagrant up
vagrant ssh -c /vagrant/instalar
```

## Montando o ambiente numa instalação Ubuntu

```bash
./instalar
```

## Acessando a aplicação

```
firefox http://localhost:$SISLEGIS_PORT/sislegis
```
