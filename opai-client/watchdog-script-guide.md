# 🐶 Watchdog Script Guide

The Watchdog script will automatically run every minute after logging in. We recommend that you update to the latest version of the client to support more features.

{% hint style="danger" %}
For security reasons, we only allow device owners to set up this feature.
{% endhint %}

{% hint style="success" %}
Please upgrade your OPAI Client to 0.5.3 or newest. \
Please run your OPAI client with "--watchdog" to enable this feature.
{% endhint %}

{% hint style="info" %}
Note: You need to restart the OPAI client if re-set the script to make it effect.
{% endhint %}

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption><p>You can setup watchdog script on Settings page.</p></figcaption></figure>

Let's start with a basic sample:

```sh
echo "Hello World";
```

This will make your worker execute once every minute and output "Hello world". This script can be executed on any operating system.

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Different operating systems support different commands. In Linux and MAC, you can use shell scripts. In Windows, the supported commands are different.
{% endhint %}

Let's try some more complex scripts in Ubuntu:

```sh
current_ip=$(curl -s ip.me);
if [ "$current_ip" != "" ]; then
  echo "Your IP:" $current_ip
fi
```

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

We encourage you to share your scripts in the community to help more users better maintain their devices.
