# QubeOS screencapture-to-vm
A script tool that takes screen shoots from dom0 and copy it to the qubevm that has an active window in the moment you run the script.


### Instalation

First you must grab the script, so on a trusted running qube open up a terminal and, if you have git just run:


```bash
  git clone git@github.com:lemyskaman/screencapture-to-vm.git
  cd screencapture-to-vm

```

Then you need to copy the script to your Dom0 system, take in consideration that you must handle all copy to Dom0 carefully, there are some know security issues copiying from vms to dom0.

So on a Dom0 terminal just run:

```bash

qvm-run --pass-io <the-vm-where-you-download-it> 'cat /path/to/the/screencapture-script' > /path/to/the/screencapture-script

```

Then add the keyboard shortcut to run from your qubeos

