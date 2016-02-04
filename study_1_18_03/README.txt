For this to work, you need to clone the
following repo into this directory:
git clone git@github.com:jbkowalkowski/AnalysisWork.git

to do a test run:
docker run --rm -it -v /mnt/disk1/scratch/jbk/:/scratch centos67-study_1_18_03_e9-prof

to build and push this container:
docker build -t centos67-study_1_18_03_e9-prof .
docker tag -f <IMAGE ID> jbkowalkowski/centos67-study_1_18_03_e9-prof:latest
docker push jbkowalkowski/centos67-study_1_18_03_e9-prof:latest
