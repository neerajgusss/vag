# Vagrant

The LAB was oriented to help us get through vagrant product which helps us building and managing virtual environments generally based on software development. This lowers development environment setup time.
  The major components comprise Box which is the a packaged environment in Vagrant. A provider, which runs the VM in. It is the local or container location. A provisioner which describes how the VM environment is setup.
  Now, there are different commands in order that have been perfomred sequentilly to run the VMs in a stable and genuine manner. First is "vagrant init" to initialise the directory to be the root directory which creates a configuration file with default commmands ready to be instructed to be compiled as soon as we uncomment the commands and start the vagrant by using the command "vagrant up" which starts the VM with predefined config commands in config file Vagrantfile. "vagrant status" tells about the status about the VM/VMs in the config file contained in the directory we have initialised. "vagrant halt" stops the vagrant thus VMs while "vagrant suspend" suspends and "vagrant resume" resumes the VM states.
    The vagrant runs the commands in the vagrantfile sequentially. The different sections in the file are :
        1.	config.vm.box - which defines the operating system
        2.  config.vm.provider – defines virtual box
        3.  config.vm.network -   defines how host sees the box ( Let's us choose the private and local addressing of reading the HTML)
        4.  config.vm.synced_folder – defines local host directories and location inside the VM which are synced to each other thus any change in the local directory will bring the same change in the location configured inside the VM.
        5.  config.vm.provision – The setup we want that explains the source script through which vagrant performs the operatons inside the VMs.
