My patched dwm build

https://codeberg.org/mok0/suckless-patches

Install

sudo make clean install

Modify

Add patches to dwm.yaml

uv init

uv add pyyaml

uv run suckless-patches.py dwm.yaml

This will download and generate a quilt series file

quilt push

You will probably get a couple rejected files 

quilt push -f

To apply the patch, then manually patch the rejected
files.

quilt refresh 

To refresh the patch after modification

quilt pop -a 

To remove all patches

quilt top

To see the currently applied patch

A better tutorial is available at

https://codeberg.org/mok0/suckless-patches

Patches:

xrdb (colors)

cfacts + vanitygaps

alpha

custom refresh rate

swallow

attachaside


