# Bookie Vagrant

Use [Vagrant](http://www.vagrantup.com/) to get [Bookie](https://github.com/mitechie/Bookie) up and running in a local VM.

## Usage

1) Clone bookie-vagrant

```
git clone https://github.com/fitztrev/bookie-vagrant.git
cd bookie-vagrant
```

2) *Optional:* Fork [Bookie](https://github.com/mitechie/Bookie) and use your own repo instead of mitechie's.

```
git clone git@github.com:<YOUR_USERNAME>/Bookie.git
```

3) Start + provision the VM.

```
vagrant up
```

This will start Bookie at [http://127.0.0.1:6543](http://127.0.0.1:6543).

The default credentials are **admin**/**admin**.