#Artifactory Cloudformation

This template stands up an Artifactory Pro server, with Oracle Java JDK.
Chef-Solo is installed and configured, the runlist is sourced from this github repo at this stage to bypass annoying CF formatting issues and problems with ' and " not parsing correctly.  

Also, easier to update externally from the template to make a change to runlist etc, if you want to add additional things to the server build without having to modify the base template.

Much refactoring is require, but at this stage it does work and Artifactory listens on port 8081.

-- Things to Do --
- Add EBS volume for Artifactory Storage.
- Refactor static references to become parameters.
- Test the use of S3 Bucket mount for backup using fuse s3fs http://fuse.sourceforge.net/
- Decide on local nginx or seperate nginx instance for handling SSL 


