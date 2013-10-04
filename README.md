# Bookie Vagrant

Use [Vagrant](http://www.vagrantup.com/) to get [Bookie](https://github.com/mitechie/Bookie) up and running in a local VM.

## Usage

1) Clone bookie-vagrant

```
git clone https://github.com/fitztrev/bookie-vagrant.git
cd bookie-vagrant
```

2) Clone Bookie into the `bookie-vagrant` directory. Optionally, you can fork [Bookie](https://github.com/mitechie/Bookie) and use your repo here instead if you plan to develop and make any changes.

```
git clone https://github.com/mitechie/Bookie.git
```

3) Start + provision the VM.

```
vagrant up
```

This will start Bookie at [http://127.0.0.1:6543](http://127.0.0.1:6543).

The default credentials are **admin**/**admin**.