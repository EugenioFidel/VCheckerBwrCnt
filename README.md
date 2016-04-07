# VCheckerBwrCnt


VCheckerBwrCnt is a Docker container which checks if an artifact in a determinate version is located in Bower.io repositories. 

### VCheckerBwrCnt 
gets the data about the artifact from a json file with this structure

            {
		"artifact":"[artifact name]",
		"version":"[artifact version]"
	    }

 To get VCheckerBwrCnt docker container : docker pull ugenio/vcheckerbwrcnt
 
 To run the container: docker run -v [path to json file]:/usr/src/mymaven/[json name] -e "REPOSITORIES=[json name]" ugenio/vcheckerbwrcnt
