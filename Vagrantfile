Vagrant.configure(2) do |config|
  #choose which vm you are using from atlas.hashicorp.com/boxes/search
  config.vm.box = "ubuntu/trusty32"
  #set the hostname of the machine
  config.vm.hostname = "joey.be"
  #configure a forwarded port for html traffic
  #port is in use on laptop use following commands:
  # netstat -anob | findstr "8080"
  # tasklist | findstr "[above pid]"
  # taskkill /pid [pid]
  config.vm.network "forwarded_port", guest:80, host:8080
  #notify user when vagrant is up
  config.vm.post_up_message
  
  
end
