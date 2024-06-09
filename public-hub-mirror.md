---
description: OPAI.Space Hub Mirror
---

# 🐳 Public Hub Mirror

## Overview

Due to the current limiting of Docker Hub, many workers encountered code:125 problem. Therefore, we set up a public and free Hub mirror service, to help workers quickly grab the latest image.

This is a non-profit service that provides Docker Hub acceleration services for OPAI users. **Please do not abuse in other ways.**

## How to use?

{% hint style="info" %}
Replace the default image URL with **https://docker.opai.space**
{% endhint %}

On Ubuntu or macOS, create or modify /etc/docker/daemon.json:

```
{
  "registry-mirrors": [
    "https://docker.opai.space"
  ]
}          
```
