# Installation and Setup

Kubebuilder requires multiple binaries to be installed and cannot be installed with `go get`.

{% method %}

## Installing a stable release

Install kubebuilder by downloading the latest stable release from the
[github repo](https://github.com/kubernetes-sigs/kubebuilder/releases).

{% sample lang="mac" %}
```bash
version=1.0.0 # latest stable version
arch=amd64

# download the release
curl -L -O https://github.com/kubernetes-sigs/kubebuilder/releases/download/v$version/kubebuilder_$version_darwin_$arch.tar.gz

# extract the archive
tar -zxvf kubebuilder_$version_darwin_$arch.tar.gz
sudo mv kubebuilder_$version_darwin_$arch /usr/local/kubebuilder

# update your PATH to include /usr/local/kubebuilder/bin
export PATH=$PATH:/usr/local/kubebuilder/bin
```

{% sample lang="linux" %}
```bash
version=1.0.0 # latest stable version
arch=amd64

# download the release
curl -L -O https://github.com/kubernetes-sigs/kubebuilder/releases/download/v$version/kubebuilder_$version_linux_$arch.tar.gz

# extract the archive
tar -zxvf kubebuilder_$version_linux_$arch.tar.gz
sudo mv kubebuilder_$version_linux_$arch /usr/local/kubebuilder

# update your PATH to include /usr/local/kubebuilder/bin
export PATH=$PATH:/usr/local/kubebuilder/bin
```

{% endmethod %}

{% method %}

## Installing latest release from master

You can install the latest kubebuilder release built from the master. Note that
this release is not well tested, so you might encounter some bugs.

{% sample lang="mac" %}
```bash
arch=amd64

# download the release
curl -L -O https://storage.googleapis.com/kubebuilder-release/kubebuilder_master_darwin_$arch.tar.gz

# extract the archive
tar -zxvf kubebuilder_master_darwin_$arch.tar.gz
sudo mv kubebuilder_master_darwin_$arch /usr/local/kubebuilder

# update your PATH to include /usr/local/kubebuilder/bin
export PATH=$PATH:/usr/local/kubebuilder/bin
```
{% sample lang="linux" %}
```bash
arch=amd64

# download the release
curl -L -O https://storage.googleapis.com/kubebuilder-release/kubebuilder_master_linux_$arch.tar.gz

# extract the archive
tar -zxvf kubebuilder_master_linux_$arch.tar.gz
sudo mv kubebuilder_master_linux_$arch /usr/local/kubebuilder

# update your PATH to include /usr/local/kubebuilder/bin
export PATH=$PATH:/usr/local/kubebuilder/bin
```
{% endmethod %}
