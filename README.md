## docker_usage
<br>

#### 1.open and login to ubuntun
```
docker run -it ubuntu /bin/bash
```


#### 2.go int alpine for crystal
```
docker run -it alpine /bin/ash # and do somethings and exit
docker commit -a myth -m 'install crystal' 7d40949fa189 alpine_crystal # save the change to new local image  alpine_crystal
```
or
```
docker commit -a 'myth' -m 'install crystal' 19bc5431d047 ilikeorange/alpine-crystal # save the change to new local image  alpine_crystal for push
docker push ilikeorange/alpine-crystal #push the new image to dockerhub
```

#### 3.cp betweent contain and Host
```
docker cp 03d0c69f8ed5:/crystal/rr .
```

#### 4.docker search images by name
```
docker search alpine 	 # can not get alpine-crystal
docker search alpine-crys # can     get apline-crystal
```
