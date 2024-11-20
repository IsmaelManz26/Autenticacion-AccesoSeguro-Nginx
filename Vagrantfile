Vagrant.configure("2") do |config|
  config.vm.define "nginx_autenticacion" do |nginx|
    nginx.vm.box = "debian/bookworm64"
    nginx.vm.hostname = "nginx-autenticacion"
    nginx.vm.network "private_network", ip: "192.168.56.10"

    # Ejecuta el script de provisión para instalar y configurar Nginx
    nginx.vm.provision "shell", path: "provision.sh"

    # Copio mi archivo de configuración de Nginx
    #cp /vagrant/ismael /etc/nginx/sites-available/
    
  end
end
