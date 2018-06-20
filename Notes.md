# Thoughts on Process

## Components of a build right now.

* Code Commit
    * Changes here kick off the build process
* CodePipeline
    * This manages the build from step to step
* CodeBuild
    * This grabs the source code and runs the packer portion. 

## Thoughts

With the current model, there will need to be a separate code repo for each one of the AMIS that are being built. While this is not bad, it does mean that there will be duplication of work. One possible way around this is to have one repo for both the CISL2 image and the standard image.

