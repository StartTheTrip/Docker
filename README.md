# Docker
 Collection of Docker files including compose YAMLs

Useful commands:
Copy folder contents to docker container:
docker cp src_path container:dest_path
docker cp from_location container_name:/var/location/www/web

#Copy file
docker cp ./file.txt container_name:/var/location/www

#Multiple files
for file in *.txt; do docker cp $file container:/app; done

##Copy from container to host
docker cp container_name:/var/location/www/web/shop.html /home/user/to_location
