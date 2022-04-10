# Freedom Software Binaries #

This is an empty package at this time.

https://forums.whonix.org/t/policy-for-inclusion-of-compiled-software/6635

## How to install `binaries-freedom` using apt-get ##

1\. Download the APT Signing Key.

```
wget https://www.kicksecure.com/derivative.asc
```

Users can [check Whonix Signing Key](https://www.kicksecure.com/wiki/Signing_Key) for better security.

2\. Add the APT Signing Key..

```
sudo cp ~/derivative.asc /usr/share/keyrings/derivative.asc
```

3\. Add the derivative repository.

```
echo "deb [signed-by=/usr/share/keyrings/derivative.asc] https://deb.kicksecure.com bullseye main contrib non-free" | sudo tee /etc/apt/sources.list.d/derivative.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `binaries-freedom`.

```
sudo apt-get install binaries-freedom
```

## How to Build deb Package from Source Code ##

Can be build using standard Debian package build tools such as:

```
dpkg-buildpackage -b
```

See instructions.

NOTE: Replace `generic-package` with the actual name of this package `binaries-freedom`.

* **A)** [easy](https://www.kicksecure.com/wiki/Dev/Build_Documentation/generic-package/easy), _OR_
* **B)** [including verifying software signatures](https://www.kicksecure.com/wiki/Dev/Build_Documentation/generic-package)

## Contact ##

* [Free Forum Support](https://forums.kicksecure.com)
* [Professional Support](https://www.kicksecure.com/wiki/Professional_Support)

## Donate ##

`binaries-freedom` requires [donations](https://www.kicksecure.com/wiki/Donate) to stay alive!
