Using vagrant docker-images
=============

To use a built image with vagrant:

```ruby
# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.provider "docker" do |d|
    d.image = "my_image_name"
    d.has_ssh = true # Required for provisioning and 'vagrant ssh' to work.
  end
end
```
