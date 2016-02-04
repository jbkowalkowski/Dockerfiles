
to do a test run:
docker run --rm -it -v /mnt/disk1/scratch/jbk/:/scratch centos67-art_1_18_03_e9-prof

to build and push this container:
docker build -t centos67-art_1_18_03_e9-prof .
docker tag -f <IMAGE ID> jbkowalkowski/centos67-art_1_18_03_e9-prof:latest
docker push jbkowalkowski/centos67-art_1_18_03_e9-prof:latest
~                                                                    
